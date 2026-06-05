# Arabic Professional Text on Image

A professional tool to add Arabic text and logos to images with perfect Right-to-Left (RTL) support, advanced text wrapping, and a built-in collection of 21 premium Arabic fonts.

This tool solves the long-standing problem of rendering Arabic text correctly on images using Python's Pillow (PIL) library.

---

## Key Features

- 21 Professional Arabic Fonts: Automatically downloads a curated collection of high-quality Arabic fonts (e.g., Ping, Adobe Arabic, Poppins) from the cloud. No need to install them on your system.
- Perfect RTL Support: Renders Arabic text correctly from right-to-left, handling mixed text, numbers, and symbols seamlessly.
- Logo Overlay: Add and customize a logo (size, opacity, position) on your image.
- Advanced Text Styling: Full control over font, size, color, stroke (outline), and position.
- Smart Line Wrapping: Text automatically wraps to fit within the image boundaries.
- Intelligent Text Segmentation: Separates Arabic, English, numbers, and symbols to apply correct styling and direction for each.
- Bracket & Punctuation Handling: Properly processes brackets `(Hello)` to `(olleH)` and adjusts punctuation placement for an Arabic layout.
- Easy-to-use Interface: Provides a clean and intuitive interface built with Gradio.

---

## How It Works (Under the Hood)

This tool tackles the core challenges of Arabic typography in PIL:

1.  Font Management: When the app starts, it downloads the 21 Arabic fonts from a Supabase cloud storage to a temporary local folder, making them available for use.
2.  Text Analysis: The input text is analyzed character by character to identify Arabic, English, numbers, and symbols.
3.  RTL Reordering: Arabic segments are identified and reversed to render correctly from right to left.
4.  Glyph Shaping & Drawing: Each segment is drawn with its appropriate font, direction, and styling (color, stroke).

---

## Technologies Used

- Python: The core programming language.
- Gradio: For building the interactive web interface.
- Pillow (PIL): For all image processing and text rendering.
- Requests: To download the font files from the cloud.

---
