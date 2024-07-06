# COVID Bed Slot Booking System

## Overview

The COVID Bed Slot Booking System is a web-based application designed to manage and book hospital beds during the COVID-19 pandemic. The system has three distinct login portals: Admin, Hospital, and Patient User, each with specific functionalities to ensure efficient management and allocation of hospital resources.

## Features

### Admin Login
- **Credentials:** 
  - Username: admin
  - Password: admin
- **Functionalities:**
  - Add hospital information.
  - Provide login credentials to hospital owners.

### Hospital Login
- **Functionalities:**
  - Login using credentials provided by the admin.
  - Add and update hospital data, including bed availability and other hospital information.

### Patient User Login
- **Functionalities:**
  - Register user details.
  - Select hospitals with available beds.
  - Book bed slots using SRFID (Smart Radio Frequency Identification).

### Additional Features
- Automatic triggers and stored procedures are implemented internally for efficient data handling and updates.

## Installation

To set up the project locally, follow these steps:

1. Open the command prompt.
2. Install the required modules using the following commands:
   ```bash
   pip install flask
   pip install Flask-SQLAlchemy
   pip install Flask-Mail
   pip install mysqlclient
   pip install Flask-Login
   ```

## Usage

1. **Admin:**
   - Login with the provided credentials.
   - Add hospitals and generate credentials for hospital owners.

2. **Hospital Owner:**
   - Login with the credentials provided by the admin.
   - Update hospital information, including bed availability.

3. **Patient User:**
   - Register on the platform.
   - Select a hospital with available beds.
   - Book a bed slot using SRFID.

## Project Structure

- **Admin Module:** Manages hospitals and credentials.
- **Hospital Module:** Manages hospital data and bed availability.
- **Patient User Module:** Manages user registrations and bed bookings.

## Technologies Used

- **Backend:** Flask, Flask-SQLAlchemy, Flask-Mail, Flask-Login, mysqlclient
- **Database:** MySQL
- **Frontend:** HTML, CSS

## License

This project is licensed under the MIT License. See the LICENSE file for more details.

---

