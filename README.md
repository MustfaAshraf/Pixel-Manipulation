# Pixel Manipulation Algorithm

Welcome to the Pixel Manipulation Algorithm project! This repository contains a Python implementation for encrypting and decrypting images using pixel manipulation techniques with the PIL (Python Imaging Library) and NumPy.

## Overview

This project demonstrates how to manipulate pixels in images to achieve encryption and decryption. It provides two main functions: `encrypt_image` and `decrypt_image`, which utilize the PIL library to read, process, and save images as NumPy arrays. The encryption process involves applying bitwise XOR operations with a user-defined key to each pixel value, ensuring secure transformation of image data.

## Features

- **Encryption**: Encrypt images by XORing each pixel with a specified key.
- **Decryption**: Decrypt previously encrypted images using the same key to restore the original image.
- **Flexible**: Works with various image formats supported by PIL (e.g., PNG, JPEG).

## Algorithm Details

### Encryption

The `encrypt_image` function:
1. Loads an image from the specified path using PIL.
2. Converts the image to a NumPy array for efficient pixel-level operations.
3. Applies a bitwise XOR operation with the encryption key to each pixel value.
4. Converts the modified NumPy array back to an image and saves it as 'encrypted_image.png'.

### Decryption

The `decrypt_image` function:
1. Opens the encrypted image file using PIL.
2. Converts the image to a NumPy array.
3. Applies a bitwise XOR operation with the same key used for encryption to restore each pixel value.
4. Saves the decrypted image as 'decrypted_image.png'.

## Usage

To encrypt and decrypt images:
1. Run the `pixel_manipulation.py` script.
2. Enter the path of the image file to be encrypted.
3. Provide an encryption key (an integer).
4. The program will output the encrypted image as 'encrypted_image.png' and subsequently decrypt it to 'decrypted_image.png'.

## Example

```plaintext
Enter the path of the image file: example_image.png
Enter the encryption key (an integer): 12345

Image encrypted and saved as 'encrypted_image.png'.
Image decrypted and saved as 'decrypted_image.png'.
```
## Contributing
Contributions are welcome! Please feel free to fork this repository, make improvements, and submit pull requests. For major changes, please open an issue first to discuss the proposed modifications.

Enjoy exploring the fascinating world of image encryption and manipulation! 🌟🖼️
