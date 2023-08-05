# Library Management System Using Java Swings

The "Library Management System" is a Java-based desktop application that provides a simple graphical user interface to manage and organize books in a library. It allows users to add, view, edit, and delete book records. The application uses Java Swing for the graphical interface and employs an ArrayList to store the book records in memory.

## Technical Approach

### Graphical User Interface (GUI)

The GUI is implemented using Java Swing, a standard Java library for creating desktop applications with graphical components. The `Library_management` class extends `JFrame`, which represents the main application window. Inside the window, we use various Swing components such as `JLabel`, `JTextField`, `JButton`, and `JTable` to create a user-friendly interface for book management.

### Data Storage

The book records are stored in an `ArrayList<String[]>` named `books`. Each book is represented as an array of strings containing the following information:

1. Book ID
2. Book Title
3. Author
4. Publisher
5. Year of Publication
6. ISBN (International Standard Book Number)
7. Number of Copies

When a new book is added, its details are collected from the input fields and stored as a new array in the `books` list. Similarly, when a book is edited, the corresponding array is updated with the new information. When a book is deleted, its array is removed from the `books` list.

### Event Handling

The `Library_management` class implements the `ActionListener` interface to handle user interactions with buttons. The `actionPerformed` method is responsible for detecting the button clicks and executing the appropriate actions.

- **Add Button:** When the "Add" button is clicked, the method collects the book details from the input fields, creates a new book array, adds it to the `books` list, and displays a success message using a `JOptionPane`. The input fields are then cleared for the next entry.

- **View Button:** Clicking the "View" button generates a new window with a `JTable` to display all the books' records. The book details from the `books` list are formatted into a 2D array to populate the table.

- **Edit Button:** The "Edit" button prompts the user to input the Book ID of the book they want to edit. If the Book ID is found, the corresponding book array is updated with the new information provided by the user. A success message is displayed, and the input fields are cleared.

- **Delete Button:** When the "Delete" button is clicked, the user is prompted to enter the Book ID of the book they want to delete. If the Book ID matches a record in the `books` list, that book is removed, and a success message is displayed. The input fields are also cleared.

- **Clear Button:** The "Clear" button resets all input fields, making it easier for users to enter new book details without manually erasing previous data.

- **Exit Button:** Clicking the "Exit" button terminates the application.

## How to Use

1. Launch the application by running the main method of the `Library_management` class.
2. The main window of the application will appear with input fields to add book details and buttons to perform various actions.
3. Enter the necessary book information into the input fields and click the "Add" button to add a new book.
4. Click the "View" button to display a table with all the books currently in the library.
5. To modify a book's information, click the "Edit" button, enter the Book ID of the book you want to edit, and provide the updated details in the input fields.
6. To remove a book from the library, click the "Delete" button, enter the Book ID of the book you want to delete, and confirm the deletion.
7. To clear all input fields, click the "Clear" button.
8. To exit the application, click the "Exit" button or close the window using the standard window close button.

## Technical Limitations

As of the current version, the "Library Management System" is a basic standalone application designed for single-user interactions. It does not support features like user authentication, database integration for data persistence, or advanced search capabilities. Additionally, the book records are stored in memory, which means that data will be lost once the application is closed. Future versions of the project could potentially address these limitations and introduce more sophisticated functionalities, such as using a database for data storage and implementing user authentication for multiple users.

## GitHub Repository

The project is hosted on GitHub at: [ChetahCodes21](https://github.com/CheetahCodes21/Java-Library-Management-System.git)

## How to Contribute

Thank you for considering contributing to the "Library Management System" project! We appreciate your efforts to make the application better for everyone. There are several ways you can contribute:

1. **Report Issues:** If you encounter any bugs, errors, or unexpected behavior while using the application, please report them by opening an issue on GitHub. Make sure to provide detailed steps to reproduce the issue and any relevant information about your system setup.

2. **Feature Requests:** If you have an idea for a new feature or improvement to add to the project, feel free to submit a feature request as an issue on GitHub. We value user feedback and ideas for enhancing the application's capabilities.

3. **Code Contributions:** If you're a developer, you can contribute by implementing new features, fixing bugs, or optimizing existing code. Fork the repository, create a new branch, and submit a pull request with your changes. Please follow the coding style and conventions used in the project.

4. **Documentation:** Improving the project's documentation is a valuable contribution. You can help by updating the README.md file, adding inline comments in the code, or writing new documentation for specific functions or classes.

5. **Testing:** Thoroughly testing the application is crucial for ensuring its stability and reliability. You can help by writing and running test cases, as well as reporting the results.

6. **Translations:** If you are fluent in multiple languages, consider translating the user interface into other languages to make the application more accessible to a global audience.

7. **User Support:** Engage with other users and contributors on GitHub by providing helpful answers to questions, assisting with troubleshooting, and sharing your experiences with the application.

8. **Refer the [Code of Conduct](CODE_OF_CONTRIBUTION.md)**


---
Feel free to customize and update the README.md with any additional information, such as installation instructions, troubleshooting, contribution guidelines, or project screenshots, to make it more informative and user-friendly for potential contributors and users.
-[ChetahCodes21](https://github.com/CheetahCodes21)
