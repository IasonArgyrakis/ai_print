# ai_print

# File Content Extractor Script

This script extracts and concatenates the contents of files into a single output file. It supports both individual files and directories (with a recursive option).

## Features
- Extracts contents of a single file.
- Recursively processes all files in a directory.
- Outputs results to a `.4ai` file named after the input file or directory.

## Installation (Global Setup)
To install the script globally from GitHub Gist:

1. Download the script:
   ```bash
   sudo curl -o /usr/local/bin/ai_print  https://raw.githubusercontent.com/IasonArgyrakis/ai_print/refs/heads/main/ai_print
   ```

2. Make it executable:
   ```bash
   sudo chmod +x /usr/local/bin/ai_print
   ```

3. Now you can use the command `ai_print` from anywhere in your terminal.

## Usage

### Extract contents of a single file:
```bash
ai_print <filename>
```
This will create an output file named `<filename>.4ai` containing the file's content.

### Extract contents of all files in a directory:
```bash
ai_print -r <directory>
```
This will process all files in the directory and save the output to `<directory>.4ai`.

## Example

Extract a single file:
```bash
ai_print myfile.txt
```
Output saved to `myfile.txt.4ai`.

Extract all files in a directory:
```bash
ai_print -r myfolder
```
Output saved to `myfolder.4ai`.

## Notes
- Ensure you have the necessary permissions to read the files you are processing.
- The script will overwrite any existing `.4ai` file with the same name.

## License
This script is provided as-is with no warranty. Use at your own risk.

