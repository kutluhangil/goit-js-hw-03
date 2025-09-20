<h1>JavaScript Homework 3 — Arrays and Functions</h1>

<p><strong>Topic:</strong> Arrays (Diziler) and Functions</p>

<h2>Overview</h2>
<p>
Are you confident with arrays and functions? We believe you will succeed! 🚀 <br>
Step by step, we are climbing to new levels! 🧗‍♂️
</p>

<p>By the end of this module, you should understand:</p>
<ul>
  <li>How arrays work</li>
  <li>Basic array methods</li>
  <li>Using <code>for...of</code> loop to iterate over arrays</li>
  <li>Working with functions and parameters</li>
  <li>The difference between global and block scope</li>
</ul>

<p>Now it’s time to put these skills into practice and review the previous material.</p>

<h2>Homework Instructions</h2>
<ol>
  <li>Create a new repository named <code>goit-js-hw-03</code> and clone it to your computer.</li>
  <li>Inside the <code>goit-js-hw-03</code> folder, follow the structure exactly as shown in the scheme.</li>
  <li>Complete each task in its corresponding file.</li>
  <li>Format your code with Prettier and make sure the console shows no errors or warnings when running the live page.</li>
  <li>Submit your homework with two links: repository (source code) and GitHub Pages live page.</li>
</ol>

<h2>Tasks</h2>

<h3>Task 1 — Slug Creator</h3>
<p>
Write a function <code>slugify(title)</code> that takes the title of an article and returns the slug.
A slug is:
</p>
<ul>
  <li>Always lowercase</li>
  <li>Words separated by a dash (<code>-</code>)</li>
</ul>

<p><strong>Example checks:</strong></p>
<pre>
slugify("Arrays for begginers") ➝ "arrays-for-begginers"
slugify("English for developer") ➝ "english-for-developer"
slugify("Ten secrets of JavaScript") ➝ "ten-secrets-of-javascript"
slugify("How to become a JUNIOR developer in TWO WEEKS") ➝ "how-to-become-a-junior-developer-in-two-weeks"
</pre>

<p><strong>Neuronics Solution:</strong></p>
<pre>
function slugify(title) {
  return title.toLowerCase().split(" ").join("-");
}
</pre>

<hr>

<h3>Task 2 — Array Composition</h3>
<p>
Write a function <code>makeArray(firstArray, secondArray, maxLength)</code> that returns a new array combining the elements of both arrays. 
If the new array length exceeds <code>maxLength</code>, return only the first <code>maxLength</code> elements.
</p>

<p><strong>Example checks:</strong></p>
<pre>
makeArray(["Mango", "Poly"], ["Ajax", "Chelsea"], 3) ➝ ["Mango", "Poly", "Ajax"]
makeArray(["Mango", "Poly", "Houston"], ["Ajax", "Chelsea"], 4) ➝ ["Mango", "Poly", "Houston", "Ajax"]
makeArray(["Earth", "Jupiter"], ["Neptune", "Uranus"], 2) ➝ ["Earth", "Jupiter"]
makeArray(["Earth", "Jupiter"], ["Neptune", "Uranus"], 4) ➝ ["Earth", "Jupiter", "Neptune", "Uranus"]
</pre>

<p><strong>Neuronics Solution:</strong></p>
<pre>
function makeArray(firstArray, secondArray, maxLength) {
  const newArray = firstArray.concat(secondArray);
  if (newArray.length > maxLength) {
    newArray.length = maxLength;
  }
  return newArray;
}
</pre>

<hr>

<h3>Task 3 — Filtering an Array of Numbers</h3>
<p>
Write a function <code>filterArray(numbers, value)</code> that takes an array of numbers and a value, 
and returns a new array containing only numbers greater than <code>value</code>.
</p>

<p><strong>Example checks:</strong></p>
<pre>
filterArray([1, 2, 3, 4, 5], 3) ➝ [4, 5]
filterArray([1, 2, 3, 4, 5], 4) ➝ [5]
filterArray([12, 24, 8, 41, 76], 38) ➝ [41, 76]
</pre>

<p><strong>Neuronics Solution:</strong></p>
<pre>
function filterArray(numbers, value) {
  const newArray = [];
  for (const number of numbers) {
    if (number > value) {
      newArray.push(number);
    }
  }
  return newArray;
}
</pre>

<hr>

<h2>Submission Format</h2>
<p>
Your submission must include:
</p>
<ul>
  <li>Repository link (with source code)</li>
  <li>GitHub Pages link (live demo)</li>
</ul>
