Here's a basic structure for your project documentation that you can include in the repository. I'll detail the approach and design choices for you.

Documentation for Chemical Supplies UI Project

Project Overview

This project is a chemical supply management table UI built using HTML, CSS, and plain JavaScript. The table contains columns for various details about chemicals such as the chemical name, vendor, density, viscosity, packaging, and more. The project was created as part of an assignment for a JavaScript Web Programmer role, and it supports table sorting and basic row operations.


Features

1. Dynamic Table Creation: The table is generated dynamically using JavaScript, populated with a JSON array containing chemical data.


2. Sorting: Each column can be sorted in ascending and descending order when clicked.


3. Row Operations: There are toolbar buttons for adding, deleting, moving rows up or down, refreshing, and saving the table data.


4. Responsive Design: The UI is responsive and adapts to different screen sizes.




---

File Structure

The project consists of the following files:

index.html: The main HTML file that renders the structure of the page.

styles.css: The CSS file that contains the styling for the table and toolbar.

script.js: The JavaScript file that handles the table functionality and interaction logic.



---

Design Decisions

1. HTML Structure

The structure of the page is minimal, focusing on the table that lists chemical data. The toolbar is placed below the table for users to interact with the data (add, delete, move, save, refresh).

Bootstrap components can be integrated if needed for button designs, but basic buttons are used for simplicity.


2. CSS Styling

The table is designed to be simple and clear. The header cells are styled with a light background to differentiate them from the body rows.

:hover effects can be added to make the rows more interactive, but currently, simplicity is prioritized.


3. JavaScript Functionality

Data Handling: A sample JSON array (chemicalData) is defined in the script file. This array holds the chemical details, and the table rows are populated based on this data.

Sorting: The sortTable() function sorts the table in ascending and descending order based on the clicked column header. This function uses a basic comparison of the cell content and switches rows accordingly.

Row Operations:

Add Row: The addRow() function allows a new row to be appended at the end of the table.

Delete Row: The deleteRow() function removes the currently selected row.

Move Row Up/Down: The user can move the selected row up or down using moveRowUp() and moveRowDown() functions.

Refresh Data: Resets the table back to its original state using refreshData().

Save Data: Can be extended to save data locally using browser storage or for exporting as JSON/CSV.




---

Future Enhancements

Edit Functionality: An edit button could be added in each row, allowing users to modify cell values. A modal popup or inline editing could be implemented for this.

PWA (Progressive Web App): The application can be enhanced into a PWA by adding a service worker and enabling offline functionality.

Row Selection: Implement radio buttons or checkboxes to select rows for moving or deletion.



---

Steps to Run Locally

1. Clone the Repository:

git clone https://github.com/your-username/Chemical-Supplies-UI-Project.git


2. Open in Browser: Open index.html in any browser.


3. Host the Project:

Upload the files to a static website host such as GitHub Pages.





---

Technologies Used

HTML: For structuring the content.

CSS: For styling the table and buttons.

JavaScript: For dynamic table manipulation (sorting, adding rows, etc.).
