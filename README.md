+++markdown
# File Compression and Decompression Tool

## Overview
This project is a GUI-based application for compressing and decompressing files. It provides a user-friendly interface with essential features such as password-protection for compressed files and secure extraction of encrypted archives. The application is built using Python's `tkinter` module for the graphical interface and supports both standard and AES-encrypted zip files.

## Features
- **File Compression**:
  - Compress multiple files into a single zip archive.
  - Optionally protect the zip file with a password.
  - Uses AES-256 encryption for enhanced security.
- **File Decompression**:
  - Extract files from standard or AES-encrypted zip archives.
  - Handles password-protected files securely.
- **File Details Display**:
  - Shows detailed metadata of selected files including size, hash values (MD5 and SHA1), and timestamps.
- **User-Friendly Interface**:
  - Modern styled buttons and dynamic output area.
  - Intuitive prompts for actions like file selection, password creation, and destination folder selection.
- **Security Checks**:
  - Enforces strong password policies for encrypted zip files.

## Dependencies
- **Python Modules**:
  - `tkinter` for GUI components.
  - `hashlib` for computing hash values.
  - `pyzipper` for handling AES-encrypted zip files.
  - `os`, `time`, and `datetime` for file and system operations.

Install dependencies using pip:
```bash
pip install pyzipper
```

## How to Use

### Launch the Application
Run the main script:
```bash
python new.py
```

### Features Walkthrough

#### 1. **Compression**
   - Select files to compress.
   - Optionally, set a password for the zip file.
   - Choose a name and location for the output zip file.
   - A confirmation dialog will notify you upon successful compression.

#### 2. **Decompression**
   - Select a zip file to extract.
   - If the archive is password-protected, provide the password.
   - Choose a destination folder for extraction.
   - The application confirms successful extraction and displays the file details.

#### 3. **Clear Output**
   - Resets the output area for a clean slate.

#### 4. **Exit**
   - Gracefully exits the application.

### Interface Overview
- **Left Pane**: Contains buttons for `Compression`, `Decompression`, `Clear Output`, and `Exit`.
- **Right Pane**: Displays banners, file details, and action logs.

## Key Functions

### Compression
```python
def compression_action(output_text):
    # Handles file compression with optional password protection
```

### Decompression
```python
def decompression_action(output_text):
    # Extracts files from a zip archive, supporting password-protection
```

### File Details
```python
def display_file_details(output_text, files):
    # Displays metadata like size, hash, and timestamps for selected files
```

### Password Validation
```python
def is_strong_password(password):
    # Ensures password contains uppercase, lowercase, and numeric characters
```

## Screenshots
- **Main Interface**: A modern UI with stylish buttons and a dynamic output display.
- **Compression/Decompression Logs**: Details of actions performed, including success or error messages.

## Error Handling
- Displays detailed error messages using `messagebox` dialogs for scenarios like:
  - Weak passwords.
  - Invalid file selections.
  - Extraction errors.

## Roadmap
- Add support for more file formats.
- Include drag-and-drop file selection.
- Implement multi-threading for improved performance.

## Contributing
Feel free to open issues or submit pull requests. For significant changes, please discuss your ideas first.

## License
This project is licensed under the MIT License.

## Contact
For queries or support, contact [Your Name/Email].
+++
