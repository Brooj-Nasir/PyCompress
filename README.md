# File Compression and Decompression Tool

This project provides a GUI-based application for compressing and decompressing files with optional password protection. The application is built using Python's Tkinter library and supports strong encryption for secure file compression.

---

## Features
- **File Compression**:
  - Compress multiple files into a single `.zip` file.
  - Optional password protection with AES encryption.
  - Displays file details such as size, hashes, and timestamps before compression.
- **File Decompression**:
  - Decompress `.zip` files, including those with AES encryption.
  - Handles encrypted archives by prompting for a password.
  - Displays detailed file information after decompression.
- **Interactive GUI**:
  - Built with Tkinter for a user-friendly experience.
  - Stylish buttons and banners for better aesthetics.
- **Password Strength Validation**:
  - Enforces strong password policies for encrypted files.

---

## Prerequisites
Make sure you have the following installed:
- Python 3.6+
- Required Python libraries:
  - `tkinter`
  - `pyzipper`
  - `hashlib`

Install the dependencies using pip:
```bash
pip install pyzipper
