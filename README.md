# Tailwind CSS classes not working with CDN
This repository demonstrates a common bug encountered when using Tailwind CSS via CDN. The issue arises when Tailwind CSS classes fail to apply correctly to HTML elements, resulting in unexpected styling.  This is often due to incorrect configuration or missing steps in the setup process.

## Bug Description
The provided `index.html` file uses the Tailwind CSS CDN. However, despite including the CDN and specifying a class (`bg-red-500`), the element remains unstyled. The background color does not change to red as expected.

## Solution
The solution involves ensuring proper Tailwind CSS configuration and build process. The correct way to use Tailwind with a CDN is to include the stylesheet at the end of the body tag and not in the `<head>`. In this example, it's shown in the `<head>`, leading to the issue. Moving it to the end of the `<body>` resolves the styling problem.

## How to Reproduce
1. Clone this repository.
2. Open `index.html` in your browser.
3. Observe that the div element does not have the red background as expected.
4. Open the solution (`solution.html`) to see the resolved version.

## Bug and Solution Files
- `index.html`: Contains the code demonstrating the bug.
- `solution.html`: Contains the corrected code.