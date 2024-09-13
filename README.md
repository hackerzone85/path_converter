# Path Converter Script

This script converts Windows paths to Linux paths and vice versa for users working on WSL (Windows Subsystem for Linux).

## Usage

- To convert a Windows path to a Linux path:
  ```bash
  path_converter -w "C:\Users\mahi6\Downloads"
  ```

- To convert a Linux path to a Windows path
  ```bash
  path_converter -l "/mnt/c/Users/mahi6/Downloads"
  ```
  
- To convert a WSL Linux path to a Windows path:
  ```bash
  path_converter -u "/home/mahi/any/path"
  ```
  
- To display the help message:
  ```bash
  path_converter -h
  ```

## Installation
- Copy the script to "/usr/local/bin":
```bash
sudo cp path_converter /usr/local/bin
```
- Make the script executable:
```bash
sudo chmod +x /usr/local/bin/path_converter
```
## Author
Mahendra Gaur, PhD Scholar, Punjabi University, Patiala

## Credits
This script was created with the assistance of Microsoft Copilot.

## License
This project is licensed under the GNU General Public License v3.0 (GPL-3.0) - see the LICENSE file for details.

## Happy to help you
If you have any other questions or need further assistance, let me know! 😊
