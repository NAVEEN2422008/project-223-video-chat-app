# c223

A PDF password cracker that brute-forces encrypted documents against a wordlist.

## Features
- Detects whether a PDF is password protected (`PyPDF2`)
- Tries every word from `wordlist.txt` as the decryption key
- Prints each attempted password and a running attempt count
- Reports the found password on success or "try again" on failure

## Tech Stack
- Python 3, `PyPDF2`

## Project Structure
```
try.py                                       # working brute-force loop (PdfReader.decrypt)
"brute_force password_breaker Boiler plate.py" # older boilerplate (PdfFileReader)
wordlist.txt                                 # candidate passwords
Brute_Encrypted.pdf                          # sample encrypted PDF to test against
```

## Installation
```
pip install PyPDF2
```

## Usage
```
python try.py
```
Enter the path to an encrypted PDF; the script then iterates the wordlist until the password is found.