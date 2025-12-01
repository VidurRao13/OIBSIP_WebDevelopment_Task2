<!-- README content (HTML) - paste this into your README.md (GitHub supports raw HTML in Markdown) -->

<h1>Calculator Project</h1>

<section>
  <h2>1. Objective</h2>
  <p>
    The main objective of this project was to design and develop a fully functional, user-interactive calculator using
    <strong>HTML</strong>, <strong>CSS</strong>, and <strong>JavaScript</strong>.
  </p>
  <p>
    The calculator performs standard arithmetic operations (addition, subtraction, multiplication, division) along with
    advanced features such as <strong>percentage</strong>, <strong>square root</strong>, <strong>exponentiation</strong>,
    <strong>sign change (+/−)</strong>, double zero (<code>00</code>), and support for parentheses.
  </p>
  <p>
    Another key goal was to implement a clean user interface and ensure smooth interaction through both <em>mouse clicks</em>
    and <em>keyboard input</em>.
  </p>
</section>

<section>
  <h2>2. Tools and Technologies Used</h2>

  <h3>HTML (HyperText Markup Language)</h3>
  <ul>
    <li>Defined the structure of the calculator.</li>
    <li>Created buttons, display screens, rows, and layout divisions.</li>
  </ul>

  <h3>CSS (Cascading Style Sheets)</h3>
  <ul>
    <li>Styled the calculator UI.</li>
    <li>Used classes for buttons, screen, and layout alignment.</li>
    <li>Created a clean, responsive, and modern-looking design.</li>
  </ul>

  <h3>JavaScript</h3>
  <ul>
    <li>Implemented all calculator logic.</li>
    <li>Handled button click events and keyboard events.</li>
    <li>Managed input, expression construction, evaluation, and error handling.</li>
    <li>Added additional features such as:
      <ul>
        <li>Percentage calculation</li>
        <li>Square root</li>
        <li>Exponentiation using <code>**</code></li>
        <li>Sign toggle (<code>+/-</code>)</li>
        <li>Clear (<code>C</code>) and All Clear (<code>AC</code>)</li>
        <li>Handling parentheses</li>
        <li>Converting symbols like <code>÷</code> and <code>^</code> to valid JS syntax</li>
      </ul>
    </li>
  </ul>
</section>

<section>
  <h2>3. Steps Performed / Working of the Calculator</h2>

  <h3>Step 1: Designing the Structure (HTML)</h3>
  <ul>
    <li>A parent container was created to hold the calculator body.</li>
    <li>One display screen (<code>&lt;input&gt;</code>) was added for showing results.</li>
    <li>A <code>&lt;p&gt;</code> tag was used to show the full expression being typed.</li>
    <li>Calculator buttons were arranged in rows using multiple <code>&lt;div&gt;</code> elements.</li>
    <li>Each button was assigned classes (<code>button</code>, <code>c</code>, <code>l</code>) for functionality and styling.</li>
  </ul>

  <h3>Step 2: Styling the UI (CSS)</h3>
  <ul>
    <li>The container was centered on the page.</li>
    <li>Calculator body was styled with background, borders, padding, and spacing.</li>
    <li>Buttons were styled with hover effects, size, spacing, and grid-like alignment.</li>
    <li>The layout was made visually clean, user-friendly, and consistent.</li>
  </ul>

  <h3>Step 3: Implementing the Logic (JavaScript)</h3>

  <h4>a) Selecting Elements</h4>
  <ul>
    <li>All buttons were selected using <code>document.querySelectorAll(".button")</code>.</li>
    <li>The calculation screen and display paragraph were accessed using <code>querySelector</code> and <code>getElementById</code>.</li>
  </ul>

  <h4>b) Building the User Input</h4>
  <ul>
    <li>Every button click appends a value to a <code>calculation</code> string.</li>
    <li>The screen updates live as the user presses buttons.</li>
  </ul>

  <h4>c) Evaluating the Expression</h4>
  <p>
    A custom function <code>evaluateExpression()</code> converts visual mathematical operators into JavaScript operators:
  </p>
  <ul>
    <li><code>÷</code> → <code>/</code></li>
    <li><code>^</code> → <code>**</code></li>
    <li><code>%</code> → <code>/100</code> (handled carefully)</li>
  </ul>
  <p>
    Parentheses and decimal inputs are supported. The expression is safely evaluated using <code>Function()</code> inside a
    <code>try–catch</code> block to handle errors gracefully.
  </p>

  <h4>d) Special Buttons Functionality</h4>
  <ul>
    <li><strong>AC</strong>: Clears entire input.</li>
    <li><strong>C</strong>: Deletes the last character.</li>
    <li><strong>%</strong>: Converts current value into percentage.</li>
    <li><strong>√</strong>: Calculates square root using <code>Math.sqrt()</code>.</li>
    <li><strong>+/-</strong>: Toggles the sign of the currently entered number.</li>
    <li><strong>()</strong>: Allows grouping expressions with parentheses.</li>
    <li><strong>Keyboard Support</strong>: Pressing numbers, operators, <code>Enter</code>, <code>.</code>, and parentheses works directly from the keyboard.</li>
  </ul>

  <h4>e) Updating Display</h4>
  <ul>
    <li>The <code>&lt;p&gt;</code> element (e.g. <code>para</code>) always shows the full mathematical expression.</li>
    <li>The input box shows the current number or the final result.</li>
  </ul>
</section>

<section>
  <h2>4. Outcome / Result</h2>
  <p>
    The final output is a fully functional calculator that supports both basic and several advanced mathematical operations. Key highlights:
  </p>
  <ul>
    <li>Clean and responsive UI</li>
    <li>Real-time input display</li>
    <li>Accurate expression evaluation</li>
    <li>Support for parentheses, exponentiation, and square root</li>
    <li>Keyboard compatibility for improved user experience</li>
    <li>Robust error handling using <code>try–catch</code></li>
  </ul>
  <p>
    Overall, this project demonstrates practical usage of DOM manipulation, event handling, expression parsing/evaluation,
    and interactive UI design using core web technologies.
  </p>
</section>

<hr>

<section>
  <h2>Optional: Files / Structure</h2>
  <pre><code>
/project-root
├─ index.html       &lt;!-- calculator structure --&gt;
├─ style.css        &lt;!-- styles --&gt;
└─ script.js        &lt;!-- logic --&gt;
  </code></pre>
</section>

<section>
  <h2>License</h2>
  <p>MIT License (or choose your preferred license)</p>
</section>
