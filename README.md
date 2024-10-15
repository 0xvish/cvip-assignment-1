# Image Processing with Color Space Conversions

This project demonstrates various color space conversions and basic image manipulation using Python and NumPy. The following color spaces are covered:
- RGB to CMY
- CMY to RGB
- RGB to HSV
- HSV to RGB
- RGB to YIQ
- YIQ to RGB
- RGB to YUV
- YUV to RGB

## Prerequisites

Ensure you have the following libraries installed:
```bash
pip install numpy matplotlib opencv-python
```

## Features

### 1. Image Loading and Display
- Load and display an image using OpenCV and matplotlib in RGB format.

### 2. Image Resizing
- Resize the image to different dimensions (256x256 and 512x512).

### 3. RGB to CMY and CMY to RGB Conversion
- Convert RGB images to the CMY color space and vice versa without using OpenCV.

### 4. RGB to HSV and HSV to RGB Conversion
- Implemented the conversion of RGB images to HSV and vice versa using a custom algorithm.

### 5. RGB to YIQ and YIQ to RGB Conversion
- Conversion between RGB and YIQ color spaces.

### 6. RGB to YUV and YUV to RGB Conversion
- Conversion between RGB and YUV color spaces.

## Usage

1. **Read and Display Image in RGB**:
    - The image is read using OpenCV, which by default loads images in BGR format. It is converted to RGB and displayed.

2. **Image Resizing**:
    - Resize the loaded image to dimensions of 256x256 or 512x512.

3. **Color Space Conversions**:
    - **RGB to CMY**: The RGB values are normalized and inverted to get CMY.
    - **CMY to RGB**: Inversion of the CMY values back to RGB.
    - **RGB to HSV**: Calculate hue, saturation, and value based on the maximum and minimum RGB components.
    - **HSV to RGB**: Convert hue, saturation, and value back into RGB using the chroma and auxiliary variables.
    - **RGB to YIQ**: Convert RGB to YIQ based on the standard matrix transformation.
    - **YIQ to RGB**: Convert YIQ back to RGB using inverse matrix operations.
    - **RGB to YUV**: Apply matrix multiplication to convert RGB values to YUV.
    - **YUV to RGB**: Reverse the transformation using the YUV to RGB matrix.

## Example

### Color Conversion from RGB to YIQ

```python
# Convert an image from RGB to YIQ
yiq_image = rgb_to_yiq(rgb_image)
plt.imshow(yiq_image[..., 0], cmap='gray')  # Display Y channel
plt.show()
```

## Contribution

Feel free to contribute to this project by improving the color space conversions or adding new features!

## License

This project is licensed under the MIT License.
