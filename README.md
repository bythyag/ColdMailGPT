# Cold Email Generator

A Python-based tool for automating personalized cold emails to professors or professionals, using OpenAI's API to generate customized email text. Ideal for students or researchers reaching out for research or project opportunities.

## Features
- Automates email generation and sending via Gmail.
- Customizable email text generated by OpenAI's API.
- Supports attachments (e.g., CV or resume).
- Loads and processes professor data from Excel files for easy bulk emailing.

## Requirements

- Python 3.7+
- Gmail account with app-specific password enabled.
- Environment variables configured for credentials and OpenAI API key.
- The following libraries:
  - `smtplib`, `email.mime`, `os`, `pandas`, `tqdm`, `time`, `typing`, `dotenv`, and `openai`.

## Setup

1. **Clone the Repository**
   ```bash
   git clone https://github.com/your-username/cold-email-generator.git
   cd cold-email-generator
   ```

2. **Install Dependencies**
   Install the required packages listed in `requirements.txt`.
   ```bash
   pip install -r requirements.txt
   ```

3. **Set Up Variables**
   ```
   SENDER_EMAIL=your-email@gmail.com
   GMAIL_APP_PASSWORD=your-app-specific-password
   OPENAI_API_KEY=your-openai-api-key
   ```

5. **Configure User and Paths**
   Customize your details (e.g., name, degree, research interests) in the `user_details` dictionary and provide the path to the Excel file with professor details and your CV file (optional).

6. **Run the Script**
   ```bash
   python cold_email_generator.py
   ```

## Usage

To execute the email generation and sending process, fill in the professor details Excel file and the user information, then run the main script. This will generate and send personalized emails to each professor listed in the Excel file.

## File Structure

- `cold_email_generator.py`: Main script with the `ColdEmailGenerator` class.
- `README.md`: Project documentation.

## License

This project is licensed under the MIT License.
