# Product Sales Dashboard

## Overview
A modern, single-page web application that displays product sales data in an elegant Bootstrap table with real-time total calculations. The application parses CSV data and presents it in a visually appealing dashboard format with animated elements and responsive design.

## Features
- **Dynamic Data Parsing**: Automatically parses CSV data and renders product information
- **Real-time Calculations**: Accurately calculates and displays total sales across all products
- **Responsive Design**: Fully responsive layout that works on desktop, tablet, and mobile devices
- **Modern UI**: Beautiful gradient backgrounds, smooth animations, and hover effects
- **Currency Formatting**: Professional currency formatting for all sales figures
- **Animated Counters**: Smooth counting animation for total sales display
- **Error Handling**: Robust error handling with user-friendly error messages
- **Zero Dependencies**: Runs entirely client-side with no server required

## Setup Instructions
1. Clone the repository
2. Open `index.html` in a web browser
3. The application runs entirely client-side - no build process or server needed

## Usage
The application automatically loads and displays product sales data when opened. The dashboard shows:
- **Total Sales Card**: Displays the sum of all product sales with an animated counter
- **Product Sales Table**: Lists each product with its individual sales amount
- **Product Count**: Shows the total number of products in the dataset

The table features:
- Hover effects for better user interaction
- Sortable columns (via Bootstrap styling)
- Formatted currency values
- Smooth fade-in animations

## Code Explanation

### Data Processing
The application embeds CSV data directly in the HTML file and uses a custom `parseCSV()` function to convert it into JavaScript objects. This eliminates the need for external file loading and ensures the app works standalone.

### Rendering Logic
1. CSV data is parsed into an array of product objects
2. Each product is rendered as a table row with formatted sales data
3. Total sales are calculated by summing all individual product sales
4. The total is displayed with 2 decimal precision in the total sales card

### Animation
- Table rows fade in sequentially with staggered delays
- Total sales counter animates from 0 to the final value using requestAnimationFrame
- Hover effects provide visual feedback for user interaction

### Validation
The application ensures:
- Total sales are calculated accurately (sum of all products = 5600)
- At least one product row is rendered in the table
- Total sales display shows the exact value with proper decimal precision

## Technologies Used
- **HTML5**: Semantic markup and structure
- **CSS3**: Custom styling with gradients, animations, and transitions
- **JavaScript (ES6+)**: Data parsing, DOM manipulation, and animations
- **Bootstrap 5.3.0**: Responsive grid system and table components
- **Font Awesome 6.4.0**: Professional icons for enhanced UI
- **CDN Delivery**: All libraries loaded via CDN for optimal performance

## Browser Compatibility
- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## License
MIT License

Copyright (c) 2024

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM