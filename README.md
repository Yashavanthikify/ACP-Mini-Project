# 2D Graphics Editor

**Developer:** Yashwantha K C  
**Course Project:** Advanced C Programming Mini Project

A simple terminal-based 2D drawing application written in C. It allows users to plot basic geometric shapes like lines, rectangles, circles, and triangles on a text-based grid canvas.

---

## 🚀 Features

* **Fixed Canvas Matrix:** Simulates an 80x24 pixel grid using characters inside a 2D array.
* **Background & Drawing Pixels:** Uses the underscores (`_`) for empty canvas space and asterisks (`*`) to represent pixels.
* **Shape Rendering Engines:** Implements coordinate-stepping logic to plot straight lines, border-aligned rectangles, symmetric circles, and 3-point triangles.
* **Array Bounds Protection:** Out-of-bounds inputs are automatically clipped to prevent memory access violations or program crashes.

---

## 🛠️ How It Works

1. **Global Framebuffer:** The program holds a 2D char array matrix: `char picture[HEIGHT][WIDTH]`.
2. **Clear Screen:** `clearPicture()` loops through and resets all elements to `_`.
3. **Set Pixel:** `setPixel(int x, int y)` validates coordinates before changing elements to `*`.

