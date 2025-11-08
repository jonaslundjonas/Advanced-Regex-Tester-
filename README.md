# Advanced Regex Tester

This is a comprehensive, client-side Regex (Regular Expression) testing tool built with HTML, CSS, and JavaScript. It allows users to test and debug regular expressions in real-time, providing a suite of features for both beginners and advanced users. Because it's a single offline file, it's portable and can be used anywhere.

## Features

*   **Real-time Matching**: The tool highlights all regex matches in your test string as you type.
*   **Detailed Match Information**: A dedicated output box shows a list of all matches found, including their indices and any capture groups.
*   **Live Substitution**: Test `replace` and `replaceAll` functionality with a live preview of the output.
*   **Regex Flags**: Easily toggle common regex flags (`g`, `i`, `m`, `s`, `u`, `y`) to see how they affect the matching behavior.
*   **Pattern Library**: A dropdown menu is pre-populated with a vast library of common and useful regex patterns, from simple email validation to complex patterns for national ID numbers.
*   **File Scanner**: Users can upload text-based files (`.txt`, `.csv`, `.json`, etc.) and scan them against the current regex pattern. The tool generates and downloads a report of all matches found.
*   **Syntax Highlighting**: Matches are clearly highlighted in the text area for easy visualization.
*   **Error Handling**: The interface displays clear, real-time error messages if the regex pattern is invalid.
*   **Session Persistence**: Your work is automatically saved to your browser's local storage, so you can pick up where you left off.
*   **Responsive Design**: The layout is optimized for both desktop and mobile devices.

## How to Use

1.  **Open `index.html`**: Simply open the `index.html` file in your web browser. No server or internet connection is required.
2.  **Enter a Regex Pattern**:
    *   Type your regular expression into the "Pattern" field.
    *   Alternatively, select a pre-defined pattern from the "Load Snippet" dropdown.
3.  **Provide Test Text**:
    *   Enter the string you want to test your regex against in the "Test Text" area.
4.  **Select Flags**:
    *   Click the checkboxes to toggle flags like Global (`g`) or Case-Insensitive (`i`).
5.  **Analyze the Results**:
    *   **Live Highlighting**: Matches will be highlighted directly in the "Test Text" box.
    *   **Matches Output**: The "Matches" box will list every match and its captured groups.
    *   **Replacement Result**: If you enter a string in the "Replacement String" field, the "Replacement Result" box will show the outcome of the substitution.
6.  **Scan a File (Optional)**:
    *   Click "Choose File" to select a local text file.
    *   Click "Scan File & Download Report" to run the regex against the file's content. A `.txt` report will be automatically downloaded.

## Code Overview

All the logic for this tool is contained within the `index.html` file.

*   **HTML**: Defines the structure and layout of the user interface.
*   **CSS**: Provides the styling, adhering to a modern, dark-themed Material Design aesthetic.
*   **JavaScript**:
    *   Handles all the core logic, including real-time regex testing, DOM manipulation, and event handling.
    *   Functions are fully documented with JSDoc comments, explaining the purpose, parameters, and return values for each.
    *   Key functions include `runRegexTest()` for live matching, `scanFile()` for file processing, and `loadState()`/`saveState()` for session management.

This project is designed to be a self-contained, powerful utility for anyone working with regular expressions.
