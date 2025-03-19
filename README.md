# Video-Steganography
A video steganography project involves concealing secret data within a video file, making it appear innocuous, and is often used for confidential communication or data hiding. 


## Overview
This project implements video steganography using Python. It allows users to hide and retrieve secret messages within video frames using the Least Significant Bit (LSB) steganography technique.

## Features
- Embed secret messages inside video frames.
- Extract hidden messages from a video.
- GUI interface using Tkinter.
- Uses OpenCV for video processing.
- Uses Stegano library for LSB encoding and decoding.

## Installation
Ensure you have the following dependencies installed before running the application:

```bash
pip install opencv-python Pillow stegano
```

## Usage
### 1. Embedding a Message:
1. Run the script:
   ```bash
   python main.py
   ```
2. Click on `Browse i/p Video` to select a video file.
3. Enter the `Secret Key` and the `Secret Message`.
4. Click `Submit`, then `Start Embedding` to hide the message inside the video frames.

### 2. Extracting a Message:
1. Run the script:
   ```bash
   python main.py
   ```
2. Click on `Load Embedded video` and select the stego video.
3. Enter the `Secret Key`.
4. Click `Submit`, then `Start Extract` to reveal the hidden message.

## Project Structure
```
├── main.py  # The main script
├── Key.txt  # Stores the secret key
├── Message.txt  # Stores the message
├── Video.txt  # Stores the selected video path
├── tmp/  # Temporary storage for video frames
├── README.md  # Project documentation
```

## Notes
- The application only processes the first 50 frames of the video for steganography.
- Ensure the correct secret key is provided during extraction.

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

## License
This project is licensed under the MIT License.

## Author
Developed by Rahul Raj.
