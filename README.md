# File Sharing App

## Overview
This is a simple Python-based **HTTP file sharing application** that allows you to share files over a local network. It creates a temporary HTTP server and provides a **QR code** for easy access to shared files via a web browser.

## Features
- Serves files from the **Desktop directory** (or a specified folder)
- Generates a **QR code** for easy connection
- Automatically detects the **local IP address** for sharing
- Uses **Python's built-in HTTP server** for lightweight hosting

## Requirements
Make sure you have **Python 3** installed on your system.

### Required Python Packages
Install dependencies using:
```sh
pip install pyqrcode pypng
```

## Installation
1. **Clone this repository** (or download the script manually):
   ```sh
   git clone https://github.com/yourusername/file-sharing-app.git
   cd file-sharing-app
   ```
2. **Run the script:**
   ```sh
   python3 main.py
   ```

## How It Works
- The script starts an HTTP server on `PORT 8010`
- It finds your **local IP address**
- Generates a **QR code** containing the file server URL
- Opens the QR code image in a **web browser**
- Users on the same network can **scan the QR code** or **enter the URL** in their browser to access shared files

## Troubleshooting
- **Permission Denied Error:** Run the script with `sudo` if necessary
- **Port Conflict:** Change the `PORT` variable in `main.py` to a different number
- **QR Code Not Displaying:** Ensure `pyqrcode` and `pypng` are installed

## Future Improvements
- Add authentication for secure file sharing
- Enable file uploads
- Support for custom directories

## License
This project is licensed under the **MIT License**. Feel free to use and modify it!

---
**Author:** Your Name  
📧 Contact: your.email@example.com  
🌐 GitHub: [yourusername](https://github.com/yourusername)

