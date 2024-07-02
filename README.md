# Chrome Password Exporter

`chrome_password_exporter` is a Python script that extracts saved passwords from Google Chrome and exports them to CSV or Excel files. This tool is useful for backing up your passwords or transferring them to another password manager.

## Features

- Extracts saved passwords from Google Chrome.
- Decrypts passwords using the encryption key from Chrome's local state.
- Exports extracted passwords to CSV or Excel files.
- Includes command-line options for specifying output format and file name.

## Requirements

- Python 3.6 or higher
- `pywin32` module
- `pycryptodome` module
- `pandas` module
- `openpyxl` module (if exporting to Excel)

## Installation

1. Clone this repository:
    ```bash
    git clone https://github.com/RapidScripter/chrome_password_exporter.git
    cd chrome_password_exporter
    ```

2. Install the required modules:
    ```bash
    pip install -r requirements.txt
    ```

    Ensure your `requirements.txt` includes:
    ```text
    pywin32
    pycryptodome
    pandas
    openpyxl
    ```

## Usage

1. Run the script with the desired output format and file name:
   ```bash
   python chrome_password_exporter.py --format csv --output passwords.csv

2. OR
   ```bash
   python chrome_password_exporter.py --format excel --output passwords.xlsx

## Command-line Options

- `--format`: Specifies the output file format. Accepts csv or excel.
- `--output`: Specifies the output file name.

## Example

- `python chrome_password_exporter.py --format csv --output chrome_passwords.csv`
- This command will extract all saved passwords from Chrome and save them in a file named chrome_passwords.csv.

## Disclaimer

This script is intended for personal use only. Extracting passwords from a browser without the owner's consent is illegal and unethical. Use this tool responsibly and at your own risk.

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any improvements or bug fixes.
