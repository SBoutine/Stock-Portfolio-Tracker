# Finance - Stock Portfolio Management System

## Overview

Finance is a web-based application that allows users to manage a virtual stock portfolio. Users can check stock prices, buy and sell shares, view transaction history, and track their portfolio value. Built with Python, Flask, and SQLite, this application provides a realistic stock trading experience with real-time price lookups.

## Features

- **User Authentication**
  - Secure registration and login system
  - Password hashing for security
  - Session management

- **Stock Operations**
  - Real-time stock price lookup
  - Buy shares with virtual cash
  - Sell owned shares
  - View current portfolio with valuation

- **Financial Management**
  - Track cash balance
  - Add additional funds
  - View complete transaction history

- **Data Visualization**
  - Clean tabular display of portfolio
  - Formatted currency values
  - Transaction history tracking

## Technical Stack

- **Backend**
  - Python 3
  - Flask web framework
  - SQLite database
  - CS50 library for database operations

- **Frontend**
  - HTML5 with Jinja2 templating
  - Bootstrap for responsive design
  - Custom CSS styling

## Database Schema

The application uses a SQLite database with the following tables:

1. **users**
   - id (INTEGER PRIMARY KEY)
   - username (TEXT UNIQUE)
   - hash (TEXT)
   - cash (NUMERIC)

2. **transactions**
   - id (INTEGER PRIMARY KEY)
   - user_id (INTEGER)
   - symbol (TEXT)
   - shares (INTEGER)
   - price (NUMERIC)
   - date (TEXT)

## Installation and Setup

1. **Prerequisites**
   - Python 3.x: https://www.python.org/downloads/
   - pip package manager
   - CS50 library
   - Git (for cloning the repo)

2. **Clone the repository**
   Open your terminal and run:
   ```bash
   git clone https://github.com/SBoutine/Stock-Portfolio-Tracker.git
   cd Stock-Portfolio-Tracker

3. **Create a virtual environment**
   ```bash
   python3 -m venv venv
   source venv/bin/activate

4. **Install the dependencies**
   ```bash
   pip install -r requirements.txt
   pip install Flask cs50 Flask-Session requests


5. **Set Flask environment variables**
   On macOS/Linux:
   ```bash
   export FLASK_APP=app.py
   export FLASK_ENV=development

   On Windows:
   ```bash
   set FLASK_APP=app.py
   set FLASK_ENV=development

7. **Access the Application**
   ```bash
   flask run
   
   Open a web browser and navigate to:
   ```bash
   http://localhost:5000

   (can be something else)

## Usage
1. **Registration**
   - Create a new account with username and password
   - Initial cash balance provided

2. **Stock Operations**
   - Use the Quote feature to check current prices
   - Buy shares through the Buy interface
   - Sell owned shares via the Sell page

3. **Portfolio Management**
   - View your current holdings on the homepage
   - Check transaction history
   - Add additional funds as needed
  

## Author
**Sara Boutine**  
