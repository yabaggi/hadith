# Hadith Explorer

Hadith Explorer is a client-side web application for searching and exploring a vast collection of authentic Islamic narrations (Hadiths). Its mission is to make the profound wisdom of the Prophet's traditions easily accessible to everyone in both Arabic and English.

## About The Project

This project is a powerful tool designed for students, researchers, and anyone interested in studying the traditions of the Prophet Muhammad (peace be upon him). The interface is built to be simple, fast, and responsive, allowing users to quickly find relevant narrations across multiple books. All data is stored in local JSON files, meaning the application can be run offline without needing a dedicated backend server.

## Features

-   **Dual Language Support:** Fully bilingual interface in English and Arabic, including Right-to-Left (RTL) support.
-   **Book & Chapter Selection:** Easily navigate through different books and their respective chapters.
-   **Advanced Search & Filtering:**
    -   Full-text search in both English and Arabic content.
    -   Filter by Hadith number within a chapter.
    -   Filter narrations by their authenticity status (Sahih, Hasan, Da'eef).
    -   Adjust the number of results displayed per page.
-   **Bilingual Hadith Display:** View Hadith text in both Arabic and English using a clean, tabbed interface.
-   **Book Statistics:** The "About" page provides a summary of each collection, including the total number of chapters and hadiths.
-   **Responsive Design:** Optimized for a seamless experience on both desktop and mobile devices.
-   **Serverless Operation:** Runs entirely in the browser, no backend or database required.

## Included Book Collections

The application includes data from the following Hadith collections:

-   Sahih al-Bukhari
-   Sahih Muslim
-   Sunan Abu Dawud
-   Sunan an-Nasa'i
-   Jami` at-Tirmidhi
-   Sunan Ibn Majah
-   Muwatta Malik
-   Musnad Ahmad
-   Sunan ad-Darimi

## Getting Started

To run this application locally, no special build steps or servers are needed.

1.  **Clone the repository:**
    ```bash
    git clone <repository-url>
    ```
2.  **Navigate to the directory:**
    ```bash
    cd <repository-folder>
    ```
3.  **Open the application:**
    Open the `index.html` file in your favorite web browser.

## Project Structure

```
.
├── index.html          # The main application/search page
├── about.html          # Page with project info and book statistics
├── style.css           # All CSS styles for the application
├── books.json          # Metadata for each hadith collection
├── books-chapters.json # Maps chapters to their respective books
├── chapter-range.json  # Defines the range of hadith numbers for each chapter
└── hadiths/            # Directory containing all hadith data
    ├── bukhari/
    │   └── chapter-1.json
    └── ...
```

-   **`index.html`**: The main entry point and user interface for searching Hadiths.
-   **`about.html`**: A secondary page that provides details about the project and statistics for the included books.
-   **`style.css`**: Contains all the visual styling for both pages.
-   **`*.json` files**: These root-level JSON files provide the necessary metadata for populating the book and chapter selection dropdowns.
-   **`hadiths/`**: This directory acts as the database. It contains subdirectories for each book, which in turn contain JSON files for each chapter, holding the actual Hadith texts.
