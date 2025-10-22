# Apollo Global Management Shares Outstanding Dashboard

This project provides a single-file, responsive HTML application to display key financial data for Apollo Global Management (APO), specifically its common stock shares outstanding, sourced directly from the SEC EDGAR API.

## Features

- **Dynamic Data Display**: Fetches and displays the entity's name, maximum, and minimum common stock shares outstanding for fiscal years greater than 2020.
- **Responsive Design**: Built with Tailwind CSS for a mobile-first and visually appealing layout.
- **Client-Side Data Fetching**: Utilizes JavaScript to fetch data directly from the SEC EDGAR API (via a CORS proxy).
- **Dynamic CIK Loading**: Supports loading data for any U.S. publicly traded company by appending a CIK to the URL (e.g., `index.html?CIK=0001018724`). The page updates without a full reload.
- **Error Handling**: Gracefully handles cases where data fetching fails or CIKs are not found.

## How to Run

1.  **Save the file**: Save the `index.html` content to a file named `index.html`.
2.  **Open in Browser**: Open `index.html` in your web browser.

    *Initially, it will display data for Apollo Global Management (CIK: 0001858681).* 

## Dynamic CIK Loading

To view data for a different company, simply append `?CIK=<your_cik_number>` to the URL in your browser's address bar. For example:

`index.html?CIK=0001018724` (for Apple Inc.)

The application will automatically fetch and update the displayed information without requiring a page refresh.

## Technologies Used

-   **HTML5**: Structure of the web page.
-   **Tailwind CSS**: For all styling and responsive design.
-   **JavaScript (ES6+)**: For fetching data, processing, and dynamically updating the DOM.
-   **SEC EDGAR API**: The primary data source.
-   **AllOrigins.win**: Used as a public CORS proxy to facilitate client-side requests to the SEC API.

## License

This project is open-sourced under the MIT License. See the `LICENSE` file for full details.