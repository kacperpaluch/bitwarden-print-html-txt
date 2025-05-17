# bitwarden-print-html-txt

# Bitwarden Export Printer

A tool for viewing, filtering, and printing JSON exports from the Bitwarden password manager. It also allows exporting selected data to TXT or HTML format, facilitating the creation of a readable and secure offline backup.

## Key Features

*   **Load Bitwarden JSON Export:** Supports JSON files exported directly from Bitwarden (drag-and-drop or standard file selection).
*   **Data Filtering:**
    *   Filter items by **folders** defined in Bitwarden.
    *   Filter items by **type**: Logins, Cards, Identities, Secure Notes, SSH Keys.
    *   Option to select/deselect all folders/items or choose individually.
*   **Print Preview:** Dynamic preview of selected items in a print-ready format.
*   **Support for Various Data Types:** Displays detailed information for:
    *   **Login details:** Username, password, TOTP (with QR code generation), URIs.
    *   **Payment Cards:** Cardholder, brand, number, expiration date, CVV code.
    *   **Identities:** All standard identity fields.
    *   **Secure Notes:** Note content.
    *   **SSH Keys:** Private key, public key, fingerprint.
    *   **Custom fields:** Displays additional user-defined fields.
*   **Print Settings:** Option to print each item on a separate page (page break).
*   **Data Export:**
    *   **Export to TXT:** Saves selected items as a plain text file.
    *   **Export to HTML:** Saves selected items as an HTML file with basic formatting, preserving readability and QR codes.
*   **Privacy and Security:**
    *   Operates **entirely client-side** (in your browser).
    *   No data from your export is **sent to any server**.
    *   The code is fully open-source and available for audit.
*   **User Interface:** Simple and intuitive interface.

## Available File Language Versions

This repository contains two versions of the tool:

*   **`bitwarden_print_html_txt_PL.html`**: Version with the user interface in **Polish**.
*   **`bitwarden_print_html_txt.html`**: Version with the user interface in **English**.

Please choose the file corresponding to your preferred language.
## How to Use

1.  **Export Data from Bitwarden:**
    *   In the Bitwarden application (desktop or web), go to `Tools` -> `Export Vault`.
    *   Select the `json` file format (not `.json (encrypted)`).
    *   Enter your master password to confirm the export and download the file.

2.  **Open `print_bitwarden.html`:**
    *   Download the `print_bitwarden.html` file from this repository.
    *   Open it in your preferred web browser (e.g., Chrome, Firefox, Edge, Safari).

3.  **Load the JSON File:**
    *   Drag the downloaded `*.json` file onto the designated area ("Przeciągnij plik JSON..." / "Drag JSON file here...") or click the "Wybierz plik JSON" / "Select JSON file" button and locate the file on your disk.

4.  **Filter and Select Items:**
    *   On the left side, lists of folders and item types will appear. Select those you are interested in.
    *   On the right side (in the middle column in the desktop version), a list of items matching the filters will be displayed. Select the specific items you want to print or export.
    *   Selected items will appear in the "Podgląd wydruku" / "Print Preview" section.

5.  **Adjust Print Settings (Optional):**
    *   Click the <i class="fas fa-cog"></i> "Ustawienia wydruku" / "Print Settings" icon below the preview header.
    *   Check the "Drukuj każdy element na osobnej stronie" / "Print each item on a separate page" option if you want each entry to start on a new page.

6.  **Print or Export:**
    *   **Print:** Click the <i class="fas fa-print"></i> "Drukuj" / "Print" button in the top panel.
    *   **Export to TXT:** Click <i class="fas fa-file-alt"></i> "Eksportuj do TXT" / "Export to TXT".
    *   **Export to HTML:** Click <i class="fas fa-file-code"></i> "Eksportuj do HTML" / "Export to HTML".

## Privacy and Security

This tool has been designed with your privacy in mind:

*   **All operations** (file loading, JSON parsing, filtering, preview generation, and export) occur **locally in your browser**.
*   Your data from the Bitwarden file **never leaves your computer** and is not sent to any external server.
*   Once you close the browser tab, the data is cleared from memory.

**Remember:** Printed or exported data contains highly sensitive information. Store it in a secure place, inaccessible to unauthorized individuals!

## Dependencies

*   [Font Awesome](https://fontawesome.com/) - for icons.
*   [QRCode.js](https://github.com/davidshimjs/qrcodejs) - for generating QR codes for TOTP data.

Both libraries are loaded via CDN.

## Notes

This project was created with the assistance of AI tools: Claude and ChatGPT.