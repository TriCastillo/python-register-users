# User Registration System: Validation & Registration Demo

## Scenario and Problem Statement
You are a junior developer at a start-up tasked with building a user registration system for a mobile app. The system must validate user input (name, email, password) before creating an account. The goal is to ensure only valid, secure, and well-formatted data is accepted, improving both user experience and security.

## Dataset Description
There is no external dataset. Instead, the system simulates user registration by validating and storing user data in memory. The validation logic is based on:
- Name: Must be a string and longer than 2 characters
- Email: Must have a username, an '@' symbol, and a valid top-level domain (from a predefined list)
- Password: Must be at least 8 characters, include a capital letter, and a number

## Actions and Approach
1. **Helper Functions**: Python functions (`validate_name`, `validate_email`, `validate_password`) are provided in `scripts/python_functions.py` for input validation.
2. **Notebook Workflow**: The Jupyter notebook (`notebooks/notebook.ipynb`) demonstrates how to use these functions to:
	- Inspect function docstrings
	- Validate user input
	- Register users and handle errors
3. **Error Handling**: The notebook shows how to catch and report validation errors to the user.

## Screenshots and Examples
### Example: Valid Registration
```python
register_user("Reynaldo", "reynaldo@gmail.com", "Reynaldo3")
# Output: {'name': 'Reynaldo', 'email': 'reynaldo@gmail.com', 'password': 'Reynaldo3'}
```
### Example: Invalid Name
```python
register_user("A", "reynaldo@gmail.com", "Reynaldo3")
# Output: False
```
### Screenshot
![Registration Demo](images/img.jpg)

## Technologies Used
- Python 3
- Jupyter Notebook
- Standard Python libraries (no external dependencies)

## Project Structure
```
python-register-users/
│
├── images/
│   └── img.jpg                # Screenshot/demo image
├── notebooks/
│   └── notebook.ipynb         # Main demonstration notebook
├── scripts/
│   └── python_functions.py    # Validation helper functions
├── README.md                  # Project documentation
```

## Results and Insights
- The system successfully validates user input and prevents invalid registrations.
- Clear error messages help users correct their input.
- The modular design allows easy extension for more complex validation or storage.

## Future Work
- Integrate with a real database for persistent storage
- Add more comprehensive password and email validation
- Develop a web or mobile front-end for real user interaction
- Implement unit tests for all validation functions

## Acknowledgement
- Problem statements and/or datasets in this project were sourced from DataCamp real-world projects.

## Contact Information
For questions or collaboration, contact:
- **Your Name**: [your.email@example.com](mailto:your.email@example.com)
