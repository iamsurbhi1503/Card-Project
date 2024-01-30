# Card-Project

This script manages the storage and retrieval of user information using local storage in a web browser. It prompts the user to enter their personal details, stores the information in local storage, and displays it on an HTML card. If user information is already stored, it retrieves and displays it directly.

### How it Works

1. **Check for Stored Information:**
   - The script checks if user information is already stored in local storage using the key "userInformation."

2. **Display Existing Information or Prompt User:**
   - If user information is found, it is parsed from the local storage and displayed on the HTML card.
   - If no information is found, the `storeUserInfo()` function is called to prompt the user to enter their details.

3. **Store User Information:**
   - The `storeUserInfo()` function prompts the user to enter their first name, last name, country, phone number, state, city, and village.
   - The entered information is stored in an object called `userInfo`.
   - The user information is then converted to a JSON string and stored in local storage using the key "userInformation."

4. **Display User Information:**
   - After storing or retrieving user information, the script updates the HTML card with the user's details.

### How to Use

1. **On Page Load:**
   - When the page loads, the script checks for existing user information in local storage.
   - If found, it is displayed on the card; otherwise, the user is prompted to enter their information.

2. **Entering User Information:**
   - If prompted, the user enters their first name, last name, country, phone number, state, city, and village.

3. **Viewing User Information:**
   - The entered or retrieved user information is displayed on the HTML card.

### Notes

- **Local Storage:**
  - The user information is stored in the web browser's local storage, allowing it to persist even if the user refreshes the page or navigates away.

- **Prompting User:**
  - The `prompt` function is used to gather user input. Ensure that user interaction is allowed in your application.

- **Key Used:**
  - The key "userInformation" is used for storing and retrieving user information from local storage.

### Potential Enhancements

- **Validation:**
  - Add validation checks to ensure that the entered user information is valid.

- **Improved UI:**
  - Enhance the user interface of the HTML card for a better display of user information.

- **Clear Information:**
  - Provide an option to clear stored user information.

### Contributions

Contributions and feedback are welcome. If you encounter issues or have suggestions for improvements, feel free to open an issue or submit a pull request on the GitHub repository.

Enjoy using the User Information Storage script!
