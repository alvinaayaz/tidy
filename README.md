# tidy

Drop in a messy CSV or Excel sheet. Get back a clean one, plus a plain list of everything that changed.

**Try it:** https://alvinaayaz.github.io/tidy

## What it does
- Trims extra spaces and collapses double spaces
- Removes blank rows and exact duplicate rows (ignores upper/lower case)
- Standardizes phone numbers (you choose the country code for numbers starting with 0)
- Lowercases emails and flags invalid ones
- Lets you mark which columns are phone, email, or "leave alone"
- Reads CSV (comma, semicolon or tab) and Excel; downloads as CSV or Excel

Anything it can't fix safely is kept in the file and flagged in a `needs_attention` column. Nothing is deleted except blank rows and exact duplicates.

## Privacy
Everything runs in your browser. Your file is never uploaded anywhere.

## Known limits
- Excel files need an internet connection (the Excel reader loads from a CDN). CSV works offline.
- Only the first sheet of an Excel file is read.
- Cells are treated as text, so numbers like ratings are saved as text in the Excel download.
- Phone length checks are strictest for Pakistani (+92) numbers.

## If it breaks on your file
Open an issue or message me on LinkedIn. Describe the columns and formats, without sharing private data.

Built by Alvina Ayaz.
