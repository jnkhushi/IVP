# IMAGE AND VIDEO PROCESSING

# ASSIGNMENT-1

## Features

- Read, display, and write an image
- Convert image into PNG, TIFF, BMP, and JPEG
- Resize an image
- Convert RGB image to grayscale
- Read and display a video
- Extract frames from a video

---

# ASSIGNMENT-2

## Features

### 1. Convert a Grayscale Image into a Binary Image

- **Case 1:** Assume the mean intensity of the image as the threshold value.
- **Case 2:** Input the threshold value from the user.

### 2. Convert an RGB (Color) Image into a Grayscale Image

- **Case 1:** Convert the RGB image to grayscale by taking the mean average of the three color planes (R, G, and B).
- **Case 2:** Input the weightages of the three color planes (R, G, and B) from the user. The weightage of each plane should be a value between 0 and 1, and the sum of all three weightages must be equal to 1.

**Example:**
Weightages of R, G, and B are 0.7, 0.2, and 0.1, respectively.

---

# ASSIGNMENT-3

## Features

### 1. Draw a Border Around the Input Image

- **Case 1:** Input the width of the border in terms of pixel count and the desired border color. Apply the border to a grayscale image.
- **Case 2:** Input the width of the border in terms of pixel count and the desired border color. Apply the border to a binary image.

### 2. Image Complement

- **Case 1:** Perform image complement on a grayscale image.
- **Case 2:** Perform image complement on a binary image.

---

# ASSIGNMENT-4

## Features

### 1. Log Transform

- Enhance the input image using the Log transform.
- Assume `c = 1`.

### 2. Power Law / Gamma Transform

- Enhance the input image using the Power law/gamma transform.
- Assume `c = 1`, and input the value of `gamma` from the user.

### 3. Intensity Level Slicing (Contrast Stretching)

- Enhance the input image using Intensity level slicing (Contrast stretching).
- Obtain the input range of intensity values and the desired output range of intensity values from the user.

**Example:**
The input range of intensity values from 80 to 120 is stretched to 50–150 in the output image.

---

# ASSIGNMENT-5

## Features

### 1. Image Smoothing Using Spatial Filters

Smooth the input image using the following filters:

- **Case 1:** Averaging filter (unweighted).
- **Case 2:** Weighted filter defined by `h(x, y) = max(|x|, |y|)`.
- **Case 3:** Gaussian filter.

### 2. User-Defined Parameters

- Input the filter size from the user.
- Input additional parameters such as `sigma` for the Gaussian filter.
- Input the method of padding (e.g., replication, zero padding) from the user.

---

# ASSIGNMENT-6

## Features

### 1. Histogram Equalization

- Enhance the contrast of the input grayscale image using histogram equalization.
- Display both the original image and the equalized image.

### 2. Histogram Matching (Specification)

- Perform histogram matching of the input image with that of a reference image using histogram equalization.

---

# ASSIGNMENT-7

## Features

### 1. Image Sharpening and Edge Detection

Sharpen the input image using the following techniques:

- **Case 1:** Laplacian filter.
- **Case 2:** Gradient operators of Sobel and Canny edge detector.
- **Case 3:** Unsharp masking (obtain the blurred image using a Gaussian filter of size `5x5` and `sigma = 3`).

---

# ASSIGNMENT-8

## Features

### 1. Synthetic Noise Generation and Comparison

Generate the following types of noise using equations derived from the Probability Density Functions (PDFs) of their noise distributions, compare the output with the inbuilt `imnoise` function, and plot the histograms of the generated noise to determine the shape of each distribution:

- **Case 1:** Uniform noise.
- **Case 2:** Gaussian noise.
- **Case 3:** Erlang noise.
- **Case 4:** Exponential noise.
- **Case 5:** Rayleigh noise.

---

# ASSIGNMENT-9

## Features

### 1. Local Binary Pattern (LBP)

- Implement the Local Binary Pattern (LBP) operator on a grayscale image.

### 2. Image Denoising (Gaussian and Speckle Noise)

Denoise an input image corrupted by Gaussian and Speckle noise using a `3x3` or `5x5` window with the following filters:

- **Case 1:** Wiener filter.
- **Case 2:** Median filtering.
- **Case 3:** Gaussian filter.
- **Case 4:** Bilateral filter.

---

# ASSIGNMENT-10

## Features

### 1. Adaptive Median Filtering

- Denoise the input image using an adaptive median filter.
- Input the initial window size and maximum window size (`Smax`) from the user.
- Compare the performance of the standard median filter and the adaptive median filter using Peak Signal-to-Noise Ratio (PSNR) values.

### 2. Image Segmentation via Otsu's Thresholding

- Threshold the input grayscale image using Otsu's global thresholding method for segmentation.
