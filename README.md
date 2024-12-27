Contact Manager

Overview

The Contact Manager is a Java-based desktop application built using the Swing framework. It allows users to manage a list of contacts, including their names, phone numbers, and optional profile images. This project demonstrates the use of GUIs in Java and highlights data validation, file handling, and table manipulation.

Features

1. Add Contacts

Input fields for entering the name and phone number.

Option to upload an image for the contact.

Validates that the name is not empty and the phone number contains only digits with a minimum length of 10.

2. Delete Contacts

Allows users to delete a selected contact from the table.

Automatically updates the data in both the table and the internal list.

3. Display Contacts

Displays contacts in a table with columns for Name, Phone Number, and Image.

Supports image preview with scaled-down dimensions for better visibility.

4. Image Upload

Users can upload an image using a file chooser.

Uploaded images are displayed in the table as thumbnails (scaled to 100x100 pixels).

Installation and Setup

Prerequisites

Java Development Kit (JDK) 8 or higher.

An IDE such as IntelliJ IDEA, Eclipse, or NetBeans (optional but recommended).

Steps to Run

Clone or download the project files.

Open the project in your IDE or compile using the terminal.

javac ContactManager.java

Run the application:

java ContactManager

How to Use

Adding a Contact

Enter the Name in the text field.

Enter the Phone Number in the text field.

(Optional) Click the Choose Image button to select an image file from your computer.

Click the Add Contact button to save the contact. It will appear in the table below.

Deleting a Contact

Select a contact in the table by clicking on its row.

Click the Delete Contact button to remove the selected contact.

Code Highlights

Core Components

Contact Class: Represents a single contact with fields for name, phone number, and image path.

Swing Components: Includes JTable, JLabel, JButton, JTextField, and JFileChooser for the GUI.

Image Handling: Images are scaled to 100x100 pixels for uniform display using Image.SCALE_SMOOTH.

Validation: Ensures the name field is not empty and the phone number meets the required criteria.

Key Methods

addContact(): Validates input, adds a contact to the list and table, and resets the input fields.

deleteContact(): Deletes the selected contact from the table and the underlying data structure.

uploadImage(): Handles image selection and displays the file name.

Project Structure

|-- ContactManager.java  // Main application file

Future Improvements

Save contacts to a file and load them on application startup.

Add search functionality to filter contacts by name or phone number.

Implement editing capabilities for existing contacts.

Enhance the UI with modern libraries like JavaFX.

License

This project is free to use and distribute under the MIT License.
