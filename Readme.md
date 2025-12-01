1. Objective
The main objective of this project was to design and develop a fully functional, user-interactive calculator using HTML, CSS, and JavaScript.
The calculator performs standard arithmetic operations (addition, subtraction, multiplication, division) along with advanced features such as percentage, square root, exponentiation, sign change (+/−), double zero (00), and support for parentheses.
Another key goal was to implement a clean UI and ensure smooth interaction through both mouse clicks and keyboard input.

2. Tools and Technologies Used
HTML (HyperText Markup Language):
Defined the structure of the calculator.
Created buttons, display screens, rows, and layout divisions.

CSS (Cascading Style Sheets):
Styled the calculator UI.
Used classes for buttons, screen, and layout alignment.
Created a clean, responsive, and modern-looking design.

JavaScript:
Implemented all calculator logic.
Handled button click events and keyboard events.
Managed input, expression construction, evaluation, and error handling.
Added additional features such as:
Percentage calculation
Square root
Exponentiation using **
Sign toggle (+/−)
Clear (C) and All Clear (AC)
Handling parentheses
Converting symbols like ÷ and ^ to valid JS syntax

3. Steps Performed / Working of the Calculator:
Step 1: Designing the Structure (HTML):
A parent container was created to hold the calculator body.
One display screen (input) was added for showing results.
A <p> tag was used to show the full expression being typed.
Calculator buttons were arranged in rows using multiple div elements.
Each button was assigned classes (button, c, l) for functionality and styling.

Step 2: Styling the UI (CSS):
The container was centered on the page.
Calculator body was styled with proper background, borders, padding, and spacing.
Buttons were styled with hover effects, colors, size, spacing, and grid-like alignment.
The layout was made visually clean, user-friendly, and consistent.

Step 3: Implementing the Logic (JavaScript):
a) Selecting Elements
All buttons were selected using querySelectorAll(".button").
The calculation screen and display paragraph were accessed using querySelector and getElementById.

b) Building the User Input
Every button click appends a value to a calculation string.
The screen updates live as the user presses buttons.

c) Evaluating the Expression
A custom function evaluateExpression() converts visual mathematical operators into JavaScript operators:
÷ → /
^ → **
% → /100
Parentheses and decimal inputs are supported.
The expression is safely evaluated using Function() inside a try–catch block.

d) Special Buttons Functionality
AC: Clears entire input.
C: Deletes the last character.
%: Converts current value into percentage.
√: Calculates square root using Math.sqrt().
+/-: Toggles the sign of the current entered number.
() : Allows grouping expressions.
Keyboard Support:
Pressing numbers, operators, Enter, . and parentheses works directly from the keyboard.

e) Updating Display
The <p> tag (para) always shows the full mathematical expression.
The input box shows the current number or final result.

4. Outcome / Result:
The final output is a fully functional scientific calculator that supports both basic and advanced mathematical operations. It offers:
A clean and responsive UI
Real-time input display
Accurate expression evaluation
Support for parentheses, power, and square root
Keyboard compatibility for a better user experience
Error-free working through proper validation and try–catch handling

Overall, the project successfully demonstrates DOM manipulation, event handling, expression evaluation, and interactive UI design using core web technologies.
