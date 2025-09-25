# Password Manager 

A simple command-line Password Manager built with Python using the cryptography.fernet library for secure password encryption and decryption.


# Features 

Generate and store a secure encryption key.

Add new account credentials (account name + password).

Encrypt and store passwords safely in a text file.

View and decrypt saved passwords.

Simple menu-driven interface.


# Project Structure 
password-manager/
│── key.key             # Encryption key (auto-generated once)
│── password_manager.py # Main program file
│── passwords.txt       # Encrypted passwords storage


# How It Works

## Key Handling

A key is generated (once) and saved in key.key.

The program loads this key to encrypt and decrypt passwords.

## Adding Passwords

User enters an account name and password.

Password is encrypted and stored in passwords.txt.

## Viewing Passwords

Stored passwords are decrypted and displayed securely in the terminal.


# Example Output

Here’s a screenshot of the project running in VS Code: <img width="683" height="120" alt="output" src="https://github.com/user-attachments/assets/cee96c76-34bd-40d3-8b11-f2b60fc71075" />


# Requirements

Python 3.8+

cryptography

Install dependencies:

pip install cryptography


# Usage

Run the program:

python password_manager.py


## Choose from:

add → Add a new password

view → View saved passwords

q → Quit the program


# Git Setup & Push Instructions

If you want to upload this project to GitHub:

# Initialize git (if not already done)
git init

# Add all files
git add .

# Commit changes
git commit -m "Password Manager project with README"

# Add remote repo (replace URL with your own repo link)
git remote add origin https://github.com/Uzmaalia/Password-Manager.git

# Push to GitHub
git push -u origin master


# Security Note ⚠️

Never upload your key.key or passwords.txt files to public repositories.

Always keep your key.key file safe. Losing it means you can’t decrypt your saved passwords.
