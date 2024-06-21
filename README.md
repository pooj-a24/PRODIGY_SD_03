# PRODIGY_SD_03
### Description of the Contact Management System

This Python script implements a simple contact management system that allows users to store and manage contact information. The program provides options to add new contacts, view the contact list, edit existing contacts, and delete contacts. It uses a JSON file for persistent storage of contact data.

#### Key Components:

1. **Imports and Constants**:
   - **json**: Used for reading from and writing to the JSON file.
   - **os**: Used to check the existence of the contacts file.
   - **CONTACTS_FILE**: The name of the file where contacts are stored.

2. **Function: `load_contacts`**:
   - Checks if the contacts file exists.
   - If it exists, it reads the file and loads the contacts into a dictionary.
   - If it doesn't exist, it returns an empty dictionary.

3. **Function: `save_contacts`**:
   - Takes a dictionary of contacts and writes it to the JSON file with pretty formatting.

4. **Function: `add_contact`**:
   - Prompts the user to enter a name, phone number, and email address.
   - Adds this new contact to the contacts dictionary.
   - Saves the updated contacts dictionary to the JSON file.
   - Confirms to the user that the contact has been added.

5. **Function: `view_contacts`**:
   - Checks if there are any contacts in the dictionary.
   - If there are contacts, it prints each contact's name, phone number, and email address.
   - If there are no contacts, it informs the user that no contacts were found.

6. **Function: `edit_contact`**:
   - Prompts the user to enter the name of the contact they wish to edit.
   - If the contact exists, it prompts the user to enter new phone and email details, showing the current details as default values.
   - Updates the contact's details in the contacts dictionary.
   - Saves the updated contacts dictionary to the JSON file.
   - Confirms to the user that the contact has been updated.
   - If the contact does not exist, it informs the user.

7. **Function: `delete_contact`**:
   - Prompts the user to enter the name of the contact they wish to delete.
   - If the contact exists, it removes the contact from the dictionary.
   - Saves the updated contacts dictionary to the JSON file.
   - Confirms to the user that the contact has been deleted.
   - If the contact does not exist, it informs the user.

8. **Function: `main`**:
   - Loads the existing contacts from the file into a dictionary.
   - Displays a menu to the user with options to add, view, edit, or delete contacts, or to exit the program.
   - Depending on the user's choice, it calls the appropriate function.
   - Continues to show the menu until the user chooses to exit.

### How to Use the Script:

1. **Running the Script**:
   - Execute the script in a Python environment.
   
2. **Interacting with the Menu**:
   - The user is presented with a menu of options:
     - **1. Add Contact**: To add a new contact.
     - **2. View Contacts**: To view all contacts.
     - **3. Edit Contact**: To edit an existing contact.
     - **4. Delete Contact**: To delete a contact.
     - **5. Exit**: To exit the program.

3. **Persistent Storage**:
   - Contacts are saved to `contacts.json` file, ensuring that contact information is not lost when the program exits.

This script provides a simple yet effective way to manage contacts, demonstrating basic file handling, user input, and data management in Python.
