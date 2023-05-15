# Signup Form

**Features**

* User signup form with validation
* Secure storage of user passwords using hashing algorithms
* JWT-based authentication for user login and access control
* Token-based authentication to authorize API requests
* Password reset functionality with email notifications
* Installation and Setup

1. Clone the repository:
  git clone https://github.com/Dhruvpatel1804/signup_form.git

2. Create and activate a virtual environment:
  python3 -m venv env
  source env/bin/activate

3. Install the required dependencies:
  pip install -r requirements.txt

4. Set up the database:
  python manage.py makemigrations
  python manage.py migrate

5. Configure email settings in the settings.py file to enable password reset functionality.
  
6. Start the development server:
  python manage.py runserver
  
7. Access the application in your browser at http://localhost:8000.

**JWT Authentication**
JWT authentication allows users to obtain a token upon successful login, which they can then use to authenticate subsequent API requests. Here's how it works:
    - User provides their credentials (username and password) to the login endpoint.
    - If the credentials are valid, a JWT token is generated and returned as a response.
    - The user includes this token in the Authorization header of subsequent API requests.
    - The server verifies the token's authenticity and, if valid, grants access to the requested resources.
    - JWT authentication eliminates the need for session management on the server-side, making it scalable and suitable for stateless APIs.

**Usage**
* User Signup: Fill out the signup form with valid information to create a new user account.
* User Login: Provide your credentials to the login form. Upon successful login, you will receive a JWT token that you can use for subsequent authenticated requests.
* Password Reset: If you forget your password, click on the "Forgot Password" link. You will receive an email with a password reset link. Follow the link to reset your password.
* API Endpoints: This application also provides API endpoints for user management, such as creating users, retrieving user information, and updating user profiles. To access these endpoints, include the JWT token in the Authorization header of your requests.

![image](https://github.com/Dhruvpatel1804/signup_form/assets/97275086/e8f6d0ca-f1a5-49ee-945e-839c4c82571a)

