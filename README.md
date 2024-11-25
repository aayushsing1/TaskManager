Task Master Web App

A simple Django-based task management web application that allows users to log in using their Google account and manage personal tasks. This app also provides an admin panel for managing OAuth credentials and inviting users.

Click This Link for Images and References of this Django Web App.
https://www.canva.com/design/DAGXe0DRpbQ/AgLw6On0hImh2E9OF3XhJQ/view?utm_content=DAGXe0DRpbQ&utm_campaign=designshare&utm_medium=link&utm_source=editor


 Features

 1. Google Authentication
   - Sign Up & Login: Users can log in using their Google account for authentication.
   - OAuth Integration: Google OAuth credentials (Client ID and Secret) are integrated for secure user login.

 2. Task Management
   - Create Tasks: Users can create new tasks with a title and description.
   - View Tasks: Users can view all their tasks in a dashboard.
   - Edit Tasks: Tasks can be edited by the user to modify title, description, or other details.
   - Delete Tasks: Tasks can be deleted by users once they're no longer needed.
   - Task Details: Each task has a title and description. (You can attach images for the task interface to show users what it looks like.)

 3. Admin Panel
   - Manage Google OAuth Keys: Admin users can manage and store the Google OAuth credentials required for Google login integration.
   - Invite Users: Admins can send registration links via email to invite new users to the app.
   
 4. User Roles
   - Standard Users: After logging in, users can manage their tasks independently.
   - Admin Users: Admins have access to the admin panel to manage OAuth credentials and invite users.



 Installation Guide

1. Clone the Repository: 
   ```bash
   git clone <repository-url>
   cd <project-folder>
   ```

2. Install Dependencies:
   Ensure you have Python 3.9 or higher, then create a virtual environment and install dependencies:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   pip install -r requirements.txt
   ```

3. Set Up Google OAuth:
   - Create a project on the [Google Cloud Console](https://console.developers.google.com/).
   - Enable the Google+ API and create OAuth 2.0 credentials.
   - Add the Client ID and Client Secret to the Django settings file.

4. Database Setup:
   - Run migrations to set up the database:
     ```bash
     python manage.py migrate
     ```

5. Run the App:
   - Start the development server:
     ```bash
     python manage.py runserver
     ```
   - Visit the app at `http://127.0.0.1:8000/`.



 Screenshots

 1. Login Screen
   - A screenshot showing the Google Login button for easy authentication.

 2. Dashboard (Task Management)
   - A screenshot of the task list view with options to create, edit, and delete tasks.

 3. Admin Panel
   - A screenshot of the admin panel interface where OAuth credentials and user invitations are managed.



 How to Use

 1. Login & Register:
   - Upon visiting the site, users are prompted to log in using their Google account.
   - If they are new, they can create an account by signing up with Google.

 2. Manage Tasks:
   - After logging in, users can create new tasks, view them, edit them, or delete them from the task dashboard.

 3. Admin Features:
   - Admin users can manage Google OAuth keys and send invitations to new users through the admin panel.



 Technologies Used
   - Django: The main web framework used for building the app.
   - Google OAuth 2.0: For user authentication via Google login.
   - SQLite: Default database used for storing user and task data.
   - HTML/CSS/JavaScript: For frontend interface.
   - Bootstrap: For responsive UI design (if used).



Contributing

Feel free to fork the repository and make pull requests for improvements or bug fixes.
