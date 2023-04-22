# Pattern Authentication System

This Python code generates a pattern authentication system using a set of images. The user is presented with a set of randomly shuffled images and asked to enter the sequence of images in the correct order. If the user enters the correct sequence of images, the authentication is successful, otherwise it fails.

## Getting Started

### Prerequisites

To run this code, you will need the following:

- Python 3
- Pillow library (PIL fork)

### Installing

Install Pillow using pip:

```bash
pip install Pillow
```

### Usage

1. Clone or download the repository to your local machine.

2. Open the terminal or command prompt and navigate to the directory where the code is saved.

3. Run the script using Python:

```bash
python pattern_auth.py
```

4. The program will randomly shuffle the image files specified in the `image_files` list and generate a set of pattern images.

5. The program will display the pattern images to the user.

6. The user will enter the sequence of images in the correct order.

7. If the user enters the correct sequence of images, the authentication is successful, otherwise it fails.

## Functions

### `generate_pattern_images(image_files)`

This function takes a list of image files and generates a set of pattern images by randomly shuffling the image files and loading the resulting sequence of images using Pillow. The pattern images are then returned as a list.

### `authenticate_user(pattern_images)`

This function takes a list of pattern images and displays them to the user. The user is then prompted to enter the sequence of images in the correct order. If the user's input matches the original pattern, the authentication is successful, otherwise it fails.

## Example

The following example demonstrates how to use the `pattern_auth.py` script:

```python
# specify the image files to use for the pattern
image_files = ["AAPL", "GOOG", "MSFT", "TSLA", "AMZN", "NFLX"]

# generate the pattern images
pattern_images = generate_pattern_images(image_files)

# authenticate the user
authenticate_user(pattern_images)
```

## Author

- Allen de Koker