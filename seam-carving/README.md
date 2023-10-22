# Seam Carving Image Resizer
Seam Carving Image Resizer is an implementation of the innovative content-aware image resizing technique known as seam carving. Unlike traditional resizing methods that simply crop or scale images, seam carving intelligently preserves the essential features of an image while reducing its size. This project provides a seamless way to resize images by removing pixels along vertical or horizontal paths, ensuring the retention of important visual elements.

## How It Works
Seam carving operates through a series of steps:

### 1. Energy Calculation:
The energy of each pixel is calculated based on the differences in RGB values with its neighbors. Higher differences indicate higher energy pixels.

### 2. Seam Identification:
Dynamic programming is utilized to create a matrix representing the energy values of individual pixels. This matrix is then analyzed to identify the lowest energy path from top to bottom (vertical seam) or from left to right (horizontal seam).

### 3. Seam Removal:
The identified seam with the lowest energy is removed from the image, effectively resizing it without distorting its essential features.

## Features
* **Content-Aware Resizing:** Seam carving retains the image's critical features, such as aspect ratio and object placement.
* **Dynamic Programming:** Utilizes dynamic programming techniques for efficient energy calculation and seam identification.
* **Artistic Value:** Allows for the creation of visually appealing images by intelligently removing low-energy pixels.

## Example
The image below shows an original image, a visualization of the seam identification, and the cropped image after seam removal.
![castle1-1](https://github.com/indiatoryy/C-Projects/assets/105636722/1d5c1c2c-05e5-41bb-bde6-5731b6718625)
