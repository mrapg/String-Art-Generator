🎨 Intelligent String Art Generator 🎨
A powerful, versatile, browser-based tool that transforms any image into a beautiful and intricate string art pattern. This application not only generates a visual mockup from scratch but can also load pre-existing sequence files to provide a complete, interactive, step-by-step guide for physical assembly.

✨ Features
🌐 Two-in-One Tool:

Generate Mode: Upload any JPG, PNG, or GIF and the tool will create a unique string art pattern and build guide.

Guide Mode: Already have a pin sequence? Upload the .txt file to instantly access the interactive visual build guide without needing an image.

🧠 Intelligent Algorithm: Based on an "Intelligent Greedy" method that uses a perceptual error map (balancing image darkness and edge detection) to produce high-quality, recognizable results.

🔍 Interactive Build Guide:

Step-by-Step Visualizer: An animated canvas shows you exactly which pin to connect next, with controls to move forward and backward through the steps.

Key Statistics: Automatically calculates the total number of strings and the estimated length of thread required in both feet and meters.

📏 Realistic Mockups: Specify the physical canvas size (in inches) and thread width (in mm) to generate a proportionally accurate preview of the final artwork.

📄 High-Quality Printable Template: Generates a clean, readable, and print-ready SVG template with clearly marked tick marks and numbers to help you accurately place the pins on your board.

💾 Downloadable Sequence: Download the final pin sequence as a .txt file for easy reference while building.

💻 100% In-Browser: Runs entirely in a single index.html file. No server, no setup, no internet connection required after loading.

🚀 How to Use
The generator has two primary functions.

A) Generating New Art from an Image
Open index.html: Open the index.html file in any modern web browser (Chrome, Firefox, Safari, Edge).

Upload Image: Click the "Upload Image" button and select a picture from your computer. Portraits or images with clear subjects work best.

Adjust Parameters:

Pins: The number of nails around the frame. More pins allow for more detail.

Strings: The total number of lines to be drawn.

Canvas Size & Thread Width: The physical dimensions of your project.

Generate: Click the "Generate Artwork" button and wait for the process to complete.

Review & Build: The generated art will appear alongside the original, and the full build instructions will be displayed below.

B) Loading an Existing Build Guide
Open index.html: Open the file in your browser.

Upload Sequence: Click the "Upload Pin Sequence (.txt)" button and select a valid sequence file. The file should contain numbers separated by spaces, commas, or newlines.

Load Guide: Click the "Load Guide" button.

Build: The interactive build guide will instantly appear, ready for you to use.

⚙️ How It Works
The generator uses a sophisticated version of a greedy algorithm. Unlike basic methods, this "Intelligent Greedy" algorithm doesn't just look for the darkest areas.

Perceptual Analysis: When an image is uploaded, the tool creates a "perceptual map." It analyzes the image for both contrast (dark areas) and definition (sharp edges, found using a Sobel filter).

Weighted Decision-Making: At each step, the algorithm evaluates potential strings based on how much "perceptual improvement" they offer, considering both the need to fill in dark areas and the importance of defining key features.

Sequential Path: It builds the artwork methodically, always moving from the last pin to the next best connection, which ensures a logical and continuous final path.

This approach provides an excellent balance between speed and quality, producing great results without the long processing times of more complex global search algorithms.
