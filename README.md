# Lab Report Generator 📝

A client-side web application that generates formatted DOCX lab reports from a template. Built with vanilla HTML/JS, it features a modern UI, Nepali date integration, and automatic template handling.

## ✨ Features

*   **Zero Dependencies**: Runs entirely in the browser (Client-side).
*   **Dynamic DOCX Generation**: Fills a Word template (`.docx`) with user data.
*   **Nepali Date Picker**: deeply integrated Bikram Sambat (BS) calendar with automatic conversion to English numerals (e.g., 2082-09-13).
*   **Smart Auto-fill**: Select a "Subject" and the "Teacher Name" automatically updates.
*   **Robust Template Handling**:
    *   **Auto-Correction**: Automatically fixes common "XML corruption" issues caused by Word spell-checkers splitting placeholders.
    *   **Auto-Load**: Attempts to fetch `tempfile.docx` automatically (great for GitHub Pages).
    *   **Manual Fallback**: Lets users upload a template if the auto-load fails (e.g., local use).
*   **Professional UI**: Clean, responsive design using Inter font and modern CSS.

## 🚀 How to Use

1.  **Open the App**:
    *   **Locally**: Open `index.html` in your browser.
    *   **Online**: Visit your deployed GitHub Pages link.
2.  **Fill Details**: Enter Lab No, Title, Date, etc.
3.  **Template**:
    *   If hosted online, it loads `tempfile.docx` automatically.
    *   If offline, click "Choose File" and select your template.
4.  **Generate**: Click "Generate DOCX" to download your report instantly.

## 🛠 Deployment (GitHub Pages)

This project is perfect for GitHub Pages because it is 100% static.

1.  Create a new repository on GitHub.
2.  Upload `index.html` and your `tempfile.docx`.
3.  Go to **Settings** > **Pages**.
4.  Select `main` branch and save.
5.  Your site is now live! 🌍

## 📝 Template Guide

Your `tempfile.docx` should use these placeholders:

*   `{labno}`
*   `{labtitle}`
*   `{studentname}`
*   `{rollno}`
*   `{subject}`
*   `{teachername}`
*   `{labdate}`
*   `{submitdate}`

## 📦 Libraries Used

*   **Docxtemplater**: For generating Word documents.
*   **PizZip**: For handling zip content (docx files).
*   **FileSaver.js**: For downloading the file.
*   **Nepali Date Picker**: For the calendar interface.
*   **jQuery**: Required dependency for the date picker.
