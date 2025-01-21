Short Description:
This Python script extracts Wi-Fi profile information from a Windows machine. It retrieves SSID names and their associated passwords (if available) for all the Wi-Fi networks the machine has connected to.

Example Output:
{'ssid': 'Network1', 'password': 'password123'}
{'ssid': 'Network2', 'password': 'mywifi456'}

# Wi-Fi Profiles Extractor

**Wi-Fi Profiles Extractor** is a Python script that fetches the saved Wi-Fi network names (SSID) and their corresponding passwords (if available) from a Windows machine. This script is useful for retrieving credentials for networks you've previously connected to.

## Features

- Lists all saved Wi-Fi network profiles on the machine.
- Extracts the SSID and associated password for each profile (if available).
- The script works only on Windows-based systems.
  
## Requirements

- Python 3.x
- The script requires the `subprocess` and `re` modules, which are part of the standard Python library, so no additional installations are necessary.

## Usage

1. Clone the repository to your local machine:
   
   ```bash
   git clone https://github.com/metodiangelov/instagram_hashtag_like_bot


How It Works

    The script uses subprocess.run() to run Windows' built-in netsh command to fetch the saved Wi-Fi profiles.
    It uses regular expressions (re) to extract the SSID names and passwords from the output.
    If a Wi-Fi profile doesn't have a password, it will be skipped.

Important Notes

    This script works only on Windows machines and requires administrative privileges to access Wi-Fi profile details.
    Make sure to run the script as an administrator if needed for proper access to the profile information.

License

This project is licensed under the MIT License - see the LICENSE file for details.
