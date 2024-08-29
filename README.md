# MP3 to C Array Converter

## Description

This script converts a binary file (e.g., MP3) into a C array representation. The resulting C header file includes the binary data as a byte array and its size, making it easy to include binary data directly in your C projects.

## How It Works

1. **Read the Binary File:** The script opens the specified file in binary mode and reads its contents.
2. **Convert to C Array Format:** It then converts the binary data into a C-style byte array, where each byte is represented in hexadecimal format.
3. **Generate Header File:** The script generates a `.h` header file containing the byte array and its size.

## Requirements

- Python 3.x

## Usage

To use the script, follow these steps:

1. **Save the Script:** Copy the provided Python code into a file named `mp3_to_c_array.py`.

2. **Prepare Your MP3 File:** Make sure the MP3 file you want to convert (e.g., `game_over.mp3`) is in the same directory as the script.

3. **Run the Script:** Execute the script with Python, specifying the name of the MP3 file and the desired array name.
