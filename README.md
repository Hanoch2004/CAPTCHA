# MOTION MIRROR CAPTCHA
An interactive motion-based CAPTCHA system that requires users to mirror on-screen movements, enhancing security against bots.

Motion Mirror CAPTCHA is a motion-based, interactive CAPTCHA system built to enhance the security of login and registration forms by challenging users to identify and enter mirrored or normal characters displayed with random movement and fonts. This unique design makes it difficult for bots and automated scripts to bypass the form, offering a stronger security layer than traditional text-based CAPTCHA systems.

## Features

- Motion-based CAPTCHA challenge to detect human interaction.
- Randomized display of mirrored and normal characters.
- Custom fonts and animations to ensure each CAPTCHA is unique.
- CAPTCHA refresh option to generate a new challenge on demand.
- Strong password validation with rules enforced during registration.
- Seamless integration with login and registration pages.

## Technologies Used

- HTML5
- CSS3
- JavaScript
- PHP
- MySQL (via XAMPP)

## Project Structure

/Motion-Mirror-Captcha
│
├── db_config.php // Database connection file
├── login.html // Login page with CAPTCHA
├── login.php // PHP backend for login validation
├── register.html // Registration page with CAPTCHA and password validation
├── register.php // PHP backend for user registration
├── kou.html // Sample page demonstrating login CAPTCHA
└── README.md // Project documentation


## Setup Instructions

1. Install XAMPP or any equivalent local server.
2. Place the entire project folder into the 'htdocs' directory.
3. Set up a MySQL database and configure the connection in 'db_config.php'.
4. Start Apache and MySQL services in XAMPP.
5. Open your browser and go to:
   - `http://localhost/Motion-Mirror-Captcha/register.html` to register a new user.
   - `http://localhost/Motion-Mirror-Captcha/login.html` to log in with CAPTCHA verification.

## CAPTCHA Logic Summary

The CAPTCHA system randomly generates a combination of mirrored and normal characters. These characters are displayed with various fonts and move across the screen in a pattern to make recognition by bots difficult. The user is required to manually identify these characters and input them in the provided field to pass the verification. Incorrect identification or skipping the CAPTCHA prevents form submission.

## Password Validation Rules

During registration, passwords must meet the following criteria:

- Length between 8 to 16 characters.
- At least one uppercase letter.
- At least one lowercase letter.
- At least one numeric digit.
- At least one special character (such as @, #, $, %, etc.).

Both password and confirm password fields must match for successful registration.

## Notes

- CAPTCHA characters can be entered in any order by the user, but mirrored characters must be recognized and interpreted correctly.
- The system includes a refresh button to regenerate a new CAPTCHA if the current one is difficult to solve.
- All form validations, including CAPTCHA and password checks, happen before form submission to improve security and user experience.

## License

This project is open-source and free to use under the MIT License.
