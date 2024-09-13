# Path Converter Script

This script converts Windows paths to Linux paths and vice versa for users working on WSL (Windows Subsystem for Linux).

## Path structures in Linux and Windows
_Path Separators_
  - Windows: Uses backslashes (\) to separate directories in a path. For example, C:\Users\Name\Documents.
  - Linux: Uses forward slashes (/) to separate directories. For example, /home/name/documents1.

_Drive Letters vs. Root Directory_
  - Windows: Uses drive letters to represent different storage devices or partitions, such as C:, D:, etc. Each drive letter is a separate root.
  - Linux: Has a single root directory (/). All files and directories are organized under this root, including different storage devices, which are mounted at specific directories like /mnt or /media1.

_Case Sensitivity_
  - Windows: File and directory names are case-insensitive. For example, File.txt and file.txt would be considered the same file.
  - Linux: File and directory names are case-sensitive. For example, File.txt and file.txt would be considered different files1.

_Hidden Files_
  - Windows: Hidden files are marked with a hidden attribute and are not shown by default in file explorers.
  - Linux: Hidden files start with a dot (.). For example, .hiddenfile2.

_Directory Structure_
  - Windows: Common directories include C:\Program Files, C:\Windows, and C:\Users.
  - Linux: Uses a hierarchical directory structure with directories like /bin (binaries), /etc (configuration files), /usr (user programs), and /home (user home directories)1.
  - These differences reflect the distinct philosophies and design choices behind each operating system.

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
