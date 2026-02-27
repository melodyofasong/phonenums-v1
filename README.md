# Extract Phone Numbers from text

A little tool built for the whimsy (and to save my sanity). This script plucks Indian phone numbers out of messy text files, like OCR outputs or e-paper dumps and neatly tucks them into a CSV.

## What it does
- Scans any .txt file you point it at for phone numbers.
- Filters specifically for Indian formats (National and +91).
- De-duplicates automatically, because nobody likes seeing the same number twice.
- Exports the final list into a clean epaper_phones.csv file in your current folder.

## Getting Started
1. Prerequisites
- Python 3+
- `pip install phonenumbers`

2. Usage
- Run the script: `python phonenums.py`
- When prompted, paste the full path to your text file.
- Check your folder for **epaper_phones.csv**  , all your unique numbers will be waiting there.

## Tips & Troubleshooting
- When the script asks for a path, give it the raw path like C:\Users\Name\Desktop\file.txt.
Pro Tip: Don't wrap the path in quotes (" ") or use double backslashes (\\)—the script prefers it plain!
- Indian Numbers Only: This project is currently tuned for the Indian National Format. If it's skipping numbers, double-check if they follow the +91 or 10-digit standard.
- Where's my file? The output (epaper_phones.csv) saves directly to the directory where you ran the script.

## Built With
- [python-phonenumbers](https://github.com/daviddrysdale/python-phonenumbers) - A Python port of Google's libphonenumber.
- Standard Python csv module. 
