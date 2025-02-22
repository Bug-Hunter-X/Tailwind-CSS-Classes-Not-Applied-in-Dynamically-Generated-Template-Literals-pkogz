# Tailwind CSS Dynamic Class Application Bug

This repository demonstrates a bug related to applying Tailwind CSS classes when they are dynamically generated within JavaScript template literals.  The issue occurs because Tailwind's class parsing mechanism might not correctly interpret classes created dynamically within backticks.

## Bug Description
When using a JavaScript variable to generate a Tailwind class name within a template literal (e.g., using backticks), the class might not be correctly applied. This leads to the style not being rendered. 

## Solution
The solution involves creating a function that joins the classes with the "className" attribute or using the spread syntax directly in the JSX expression if you're using React.