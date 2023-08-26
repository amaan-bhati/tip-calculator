# tip-calculator
Tip calculator using html , css and javascript.



![Screenshot 2023-08-26 232947](https://github.com/amaan-bhati/tip-calculator/assets/94218318/05594f5a-a33f-4859-ba4e-67df191a510a)
The Tip Calculator is a simple web application that allows users to calculate the appropriate tip amount for a bill. It is built using HTML, CSS, and JavaScript, providing an easy-to-use interface for calculating tips quickly and accurately.

Features
Input field for entering the total bill amount.
Option to select the desired tip percentage (e.g., 10%, 15%, 20%).
Instant calculation of the tip amount and the total bill including the tip.
User-friendly interface with responsive design for various screen sizes.
Getting Started
These instructions will help you set up a copy of the Tip Calculator project on your local machine.

Prerequisites
To run the Tip Calculator, you need a modern web browser that supports HTML5, CSS3, and JavaScript.

Built With
HTML5 - Markup language for creating the structure of the calculator.
CSS3 - Stylesheets for designing the visual appearance of the calculator.
JavaScript - Programming language for implementing the tip calculation logic and interactivity.

JavaScript Logic
The JavaScript code in this project handles the calculation of the tip amount and the total bill. When the user enters the bill amount and selects a tip percentage, the following logic is applied:
// Get references to HTML elements
const billInput = document.getElementById('bill');
const tipSelect = document.getElementById('tip');
const tipAmountElement = document.getElementById('tip-amount');
const totalAmountElement = document.getElementById('total-amount');

// Add event listeners to input and select elements
billInput.addEventListener('input', calculateTip);
tipSelect.addEventListener('change', calculateTip);

// Function to calculate the tip and total amounts
function calculateTip() {
  const billAmount = parseFloat(billInput.value);
  const tipPercentage = parseFloat(tipSelect.value);
  
  const tipAmount = billAmount * (tipPercentage / 100);
  const totalAmount = billAmount + tipAmount;
  
  tipAmountElement.textContent = `$${tipAmount.toFixed(2)}`;
  totalAmountElement.textContent = `$${totalAmount.toFixed(2)}`;
}


Tip Calculator
Tip Calculator Preview

The Tip Calculator is a simple web application that allows users to calculate the appropriate tip amount for a bill. It is built using HTML, CSS, and JavaScript, providing an easy-to-use interface for calculating tips quickly and accurately.

Features
Input field for entering the total bill amount.
Option to select the desired tip percentage (e.g., 10%, 15%, 20%).
Instant calculation of the tip amount and the total bill including the tip.
User-friendly interface with responsive design for various screen sizes.
Getting Started
These instructions will help you set up a copy of the Tip Calculator project on your local machine.

Prerequisites
To run the Tip Calculator, you need a modern web browser that supports HTML5, CSS3, and JavaScript.

JavaScript Logic
The JavaScript code in this project handles the calculation of the tip amount and the total bill. When the user enters the bill amount and selects a tip percentage, the following logic is applied:

javascript
// Get references to HTML elements
const billInput = document.getElementById('bill');
const tipSelect = document.getElementById('tip');
const tipAmountElement = document.getElementById('tip-amount');
const totalAmountElement = document.getElementById('total-amount');

// Add event listeners to input and select elements
billInput.addEventListener('input', calculateTip);
tipSelect.addEventListener('change', calculateTip);

// Function to calculate the tip and total amounts
function calculateTip() {
  const billAmount = parseFloat(billInput.value);
  const tipPercentage = parseFloat(tipSelect.value);
  
  const tipAmount = billAmount * (tipPercentage / 100);
  const totalAmount = billAmount + tipAmount;
  
  tipAmountElement.textContent = `$${tipAmount.toFixed(2)}`;
  totalAmountElement.textContent = `$${totalAmount.toFixed(2)}`;
}



Responsive Design
The Tip Calculator is designed to be responsive on all media screens. This is achieved through the use of CSS media queries that adapt the layout and styling based on the screen size. The CSS code includes rules for different screen widths, ensuring that the calculator remains usable and visually appealing across various devices.
