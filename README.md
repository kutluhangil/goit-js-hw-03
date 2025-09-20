<h1>📘 JavaScript Homework 3</h1>

<p>This repository contains solutions for 3 tasks focused on <strong>arrays and functions</strong> in JavaScript. Each task is implemented in a separate file (<code>task-1.js</code>, <code>task-2.js</code>, <code>task-3.js</code>).</p>

<hr>

<h2>🔹 Task 1: Slug Creator (<code>task-1.js</code>)</h2>

<p>A function was written to generate a <strong>slug</strong> from a given string.<br>
Slug rules:</p>
<ul>
  <li>All characters must be lowercase.</li>
  <li>Words must be joined with a dash (<code>-</code>).</li>
</ul>

<pre><code>function slugify(title) {
  return title.toLowerCase().split(" ").join("-");
}
</code></pre>

<p>✅ <strong>Test Results</strong></p>

<pre><code>slugify("Arrays for begginers"); 
// "arrays-for-begginers"

slugify("English for developer"); 
// "english-for-developer"

slugify("Ten secrets of JavaScript"); 
// "ten-secrets-of-javascript"

slugify("How to become a JUNIOR developer in TWO WEEKS"); 
// "how-to-become-a-junior-developer-in-two-weeks"
</code></pre>

<hr>

<h2>🔹 Task 2: Array Composition (<code>task-2.js</code>)</h2>

<p>A function that merges two arrays and limits the result by <code>maxLength</code>.</p>

<pre><code>function makeArray(firstArray, secondArray, maxLength) {
  const newArray = firstArray.concat(secondArray);
  if (newArray.length > maxLength) {
    newArray.length = maxLength;
  }
  return newArray;
}
</code></pre>

<p>✅ <strong>Test Results</strong></p>

<pre><code>makeArray(["Mango", "Poly"], ["Ajax", "Chelsea"], 3); 
// ["Mango", "Poly", "Ajax"]

makeArray(["Mango", "Poly", "Houston"], ["Ajax", "Chelsea"], 4); 
// ["Mango", "Poly", "Houston", "Ajax"]

makeArray(["Mango"], ["Ajax", "Chelsea", "Poly", "Houston"], 3); 
// ["Mango", "Ajax", "Chelsea"]

makeArray(["Earth", "Jupiter"], ["Neptune", "Uranus"], 2); 
// ["Earth", "Jupiter"]

makeArray(["Earth", "Jupiter"], ["Neptune", "Uranus"], 4); 
// ["Earth", "Jupiter", "Neptune", "Uranus"]

makeArray(["Earth", "Jupiter"], ["Neptune", "Uranus", "Venus"], 0); 
// []
</code></pre>

<hr>

<h2>🔹 Task 3: Filtering an Array of Numbers (<code>task-3.js</code>)</h2>

<p>A function that filters numbers from an array, keeping only those <strong>greater than a given value</strong>.</p>

<pre><code>function filterArray(numbers, value) {
  const newArray = [];

  for (const number of numbers) {
    if (number > value) {
      newArray.push(number);
    }
  }

  return newArray;
}
</code></pre>

<p>✅ <strong>Test Results</strong></p>

<pre><code>filterArray([1, 2, 3, 4, 5], 3); 
// [4, 5]

filterArray([1, 2, 3, 4, 5], 4); 
// [5]

filterArray([1, 2, 3, 4, 5], 5); 
// []

filterArray([12, 24, 8, 41, 76], 38); 
// [41, 76]

filterArray([12, 24, 8, 41, 76], 20); 
// [24, 41, 76]
</code></pre>

<hr>

<h2>📌 Summary & Reflection</h2>

<p>Great progress! 🎉 With this homework, you strengthened your skills in <strong>arrays and functions</strong>.</p>

<p>Now you know:</p>
<ul>
  <li>How arrays work</li>
  <li>Basic array methods</li>
  <li>Iteration with <code>for...of</code> loop</li>
  <li>Writing and using functions effectively</li>
  <li>The difference between <strong>global scope</strong> and <strong>block scope</strong></li>
</ul>

<p>It’s time to reinforce this knowledge with practice and keep climbing higher 🚀</p>

<hr>

<h2>📌 Overview</h2>

<ul>
  <li><strong>Task 1:</strong> Slug creation from strings</li>
  <li><strong>Task 2:</strong> Array composition with <code>concat</code> and <code>maxLength</code> limit</li>
  <li><strong>Task 3:</strong> Filtering numbers greater than a given value</li>
</ul>
