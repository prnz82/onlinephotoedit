# Online Photo Editor

A modern, web-based photo editing application that allows users to apply filters and transformations to their images directly in the browser. Built with a focus on simplicity and performance using vanilla web technologies.

## 🚀 Overview

This Online Photo Editor provides a seamless interface for basic image manipulation. Users can upload images, adjust various visual parameters like brightness and contrast, rotate or flip the images, and finally download the results. The application is entirely client-side, ensuring privacy and speed as no data is sent to a server.

---

## ✨ Features

- **🖼️ Image Upload**: Quickly select and load any image from your local device.
- **🎨 Real-time Filters**:
  - **Brightness**: Adjust the light intensity of the image.
  - **Contrast**: Enhance the difference between dark and light areas.
  - **Saturate**: Control the intensity of colors.
  - **Invert**: Flip the colors of the image for a negative effect.
  - **Blur**: Apply a Gaussian blur effect for a soft look.
- **🔄 Transformations**:
  - **Rotate**: Rotate the image 90 degrees left or right.
  - **Flip**: Mirror the image horizontally or vertically.
- **🧹 Reset Functionality**: Easily revert all changes and go back to the original image state with a single click.
- **💾 Save & Download**: Export your edited masterpiece in high quality as a `.jpg` file.

---

## 🏗️ Architecture

The application follows a clean, modular architecture using the standard web stack:

### 1. Frontend Structure
- **HTML5**: Defines the semantic structure of the editor, including the image preview area, control panels for filters, and action buttons.
- **CSS3**: Handles the visual presentation. It uses a responsive layout, custom button styling, and smooth transitions. The editor features a modern, clean UI with a focused user experience.
- **Vanilla JavaScript**: The core logic engine of the application.

### 2. Logic & Processing
- **Image Handling**: Utilizes the `FileReader` and `URL.createObjectURL` APIs to load and display images instantly.
- **Live Preview**: Leverages CSS `filter` and `transform` properties on the `<img>` element to provide real-time, hardware-accelerated feedback as the user adjusts sliders.
- **State Management**: Maintains the current state of all filters and rotations in simple JavaScript variables, ensuring synchronization between the UI sliders and the preview.
- **Export Engine**: Uses the **HTML5 Canvas API** to render the final image. When a user clicks 'Save', the app programmatically draws the image onto a canvas, applies the corresponding filters to the canvas context, and triggers a download.

---

## 📂 Project Structure

```text
.
├── css/
│   └── style.css      # Custom styling and layout
├── js/
│   └── script.js     # Image processing and UI logic
├── images/           # Asset icons for filters and rotations
├── index.html        # Main entry point and UI structure
└── README.md         # Project documentation
```

---

## 🛠️ Technologies Used

- **HTML5**
- **CSS3** (Flexbox, Grid, Filters)
- **JavaScript** (ES6+, DOM API, Canvas API)

---

## 🚦 How to Run

1. Clone or download this repository.
2. Open `index.html` in any modern web browser (Chrome, Firefox, Safari, Edge).
3. Start editing your photos!
