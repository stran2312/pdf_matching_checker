# pdf_matching_checker
# File Hash Comparator

## Overview

This Python script, `file_hash_comparator.py`, is designed to compare the hash values of two files to determine whether they are identical. It utilizes the hashlib library to generate SHA-1 hashes of file contents and then compares these hash values.

## Prerequisites

- Python 3.x
- hashlib library

## Usage

1. Ensure you have Python 3.x installed on your system.
2. Run the script from the command line or terminal:

    ```bash
    python pdf.py
    ```

3. The script will prompt you to enter the file paths for the two files you want to compare.

4. The script will then compute the SHA-1 hash values for each file and compare them.

5. The output will indicate whether the files are identical or not.

## Code Explanation

The script performs the following steps:

1. Imports necessary libraries:
   - `hashlib` for generating hash values.
   - `SequenceMatcher` from the `difflib` module (although currently not used).

2. Defines the `hash_file` function, which takes two file names as input, reads the files in chunks, and computes the SHA-1 hash values for each file.

3. Opens and reads the content of each file in 1024-byte chunks to accommodate large files.

4. Computes the SHA-1 hash values using the `update` method.

5. Returns the computed hash values as hexadecimal strings.

6. Calls the `hash_file` function with the file paths and compares the hash values.

7. Prints whether the files are identical or not based on the hash comparison.

## Note

- The script currently uses SHA-1 for hashing. If you require a different hash algorithm, you can easily modify the script by changing the hashlib function (e.g., `hashlib.sha256()`).

- Ensure that the required files exist at the specified paths before running the script.

Feel free to adapt this script to suit your specific use case or integrate it into your projects.
