CopyEdit
<html>
  <body>
    <h1>Hello</h1>
    <p>Welcome to DOM!</p>
  </body>
</html>
DOM Structure (Visually):
Document
 └── html
     └── body
         ├── h1 → "Hello"
         └── p  → "Welcome to DOM!"
JavaScript can access and modify any of these nodes.


Java Script
1. Introduction to JavaScript
🔹 What is JavaScript?
JavaScript is a lightweight, interpreted programming language used to make web pages interactive.
It runs on the client side (in the browser) and helps with dynamic content like popups, form validations, animations, etc.
✅ 1. Inline JavaScript
Code is written directly in the HTML element’s attribute (usually onclick, onmouseover, etc.).
Example:
<button onclick="alert('Hello from inline JS!')">Click Me</button>

✅ 2. Internal JavaScript
JavaScript code is written inside a <script> tag within the HTML file, usually in the <head> or at the end of the <body>.
Example:
<!DOCTYPE html>
<html>
<head>
  <title>Internal JS</title>
  <script>
    function greet() {
      alert('Hello from internal JS!');
    }
  </script>
</head>
<body>
  <button onclick="greet()">Click Me</button>
</body>
</html>
✅ Best Practice: Place <script> before </body> for better performance.

✅ 3. External JavaScript
JavaScript code is written in a separate .js file and linked using the <script src="..."> tag.
File: script.js
function greet() {
  alert('Hello from external JS!');
}
File: index.html
<!DOCTYPE html>
<html>
<head>
  <title>External JS</title>
</head>
<body>
  <button onclick="greet()">Click Me</button>

  <script src="script.js"></script>
</body>
</html>

🧠 Summary Table
Method
Location
Use Case

Inline
Inside HTML tag
Simple actions (e.g., alerts)

Internal
Inside <script>
Page-specific logic

External
Separate .js file
Best for reusable & maintainable code
