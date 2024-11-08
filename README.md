# Temporary Mail Service

This project provides a user-friendly interface for generating and managing temporary email addresses, designed to simplify email handling while keeping user data private and secure.

## Features

- **Generate Temporary Emails**: Easily generate random email addresses with a single click. The generated email address is displayed in a read-only input field, ready to be used for temporary purposes.
- **Copy Email Address**: Copy the generated email address to the clipboard effortlessly by clicking the "Copy Email Address" button, making it convenient to paste elsewhere.
- **Load and Check Emails**: Refresh and view incoming emails associated with the temporary address. The service fetches new emails and displays them, showing the sender, subject, and content.
- **Download Attachments**: If any attachments are present in the emails, you can download them directly via generated links.
- **Dynamic Interface Initialization**: The interface automatically sets up when the `.inMail` element is detected, either on page load or dynamically when added to the DOM. This ensures seamless user experience.

## How It Works

1. The interface includes buttons for loading emails, copying the address, and generating a new temporary email address.
2. A MutationObserver monitors the DOM for the presence of the `.inMail` element and initializes the interface when detected.
3. The service interacts with the [1secmail API](https://www.1secmail.com/) to generate emails, check for new messages, and download attachments.
4. Email content and attachments are loaded and displayed in real-time, with visual feedback for user actions using SVG icons and status messages.

## Usage

- Clone the repository and open the HTML file in your browser to test the interface.
- Make sure the internet connection is active, as the service relies on API calls to 1secmail for email operations.

Enjoy seamless temporary email generation and management!
