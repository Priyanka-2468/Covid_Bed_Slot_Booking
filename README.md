# COVID Bed Slot Booking System


## Introduction
The COVID Bed Slot Booking System is designed to help hospitals and healthcare facilities manage bed availability efficiently during the COVID-19 pandemic. This system allows patients or their representatives to book beds in advance, ensuring that the hospital can manage its resources effectively and patients can receive timely care.

## Features
- **User Authentication**: Secure login and registration for users.
- **Bed Availability**: Real-time updates on bed availability.
- **Slot Booking**: Users can book available slots for COVID-19 beds.
- **Notifications**: Email and SMS notifications for booking confirmations and updates.
- **Admin Panel**: Manage bed slots, view bookings, and update availability.
- **Reports**: Generate reports on bed occupancy and booking history.

## Technologies Used
- **Programming Language**: Python
- **Web Framework**: Flask
- **Database**: MySQL
- **Authentication**: JWT (JSON Web Tokens)
- **Notifications**: Twilio for SMS, smtplib for email
- **Deployment**: Docker



## Installation
To get a local copy up and running follow these simple steps:

### Prerequisites
- Python 3.x installed
- MySQL installed
- Docker installed (for containerization)

### Clone the repository
```sh
git clone https://github.com/Priyanka-2468/covid-bed-slot-booking-system.git
cd covid-bed-slot-booking-system
```

### Set up and activate virtual environment
```sh
python -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`
```

### Install dependencies
```sh
pip install -r requirements.txt
```

### Set up environment variables
Create a `.env` file in the root directory and add the following variables:
```
DATABASE_URI=mysql+pymysql://username:password@localhost:3306/database_name
JWT_SECRET=your_jwt_secret
TWILIO_SID=your_twilio_sid
TWILIO_AUTH_TOKEN=your_twilio_auth_token
TWILIO_PHONE_NUMBER=your_twilio_phone_number
EMAIL_HOST=your_email_host
EMAIL_PORT=your_email_port
EMAIL_USER=your_email_user
EMAIL_PASS=your_email_password
```

### Set up the database
1. Log into MySQL and create a database:
    ```sql
    CREATE DATABASE covid_bed_booking;
    ```
2. Import the database schema:
    ```sh
    mysql -u username -p covid_bed_booking < covid.sql
    ```

### Run the application
```sh
python main.py
```

The application will be running on `http://localhost:5000`.

## Usage
1. **Register or Login**: Users can register for a new account or login using existing credentials.
2. **View Bed Availability**: Check the availability of COVID-19 beds.
3. **Book a Slot**: Select an available slot and confirm the booking.
4. **Receive Notifications**: Get notifications for booking confirmation and updates.
5. **Admin Panel**: (For admins only) Manage bed availability, view bookings, and generate reports.


## Contributing
Contributions are what make the open-source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/YourFeature`)
3. Commit your Changes (`git commit -m 'Add some feature'`)
4. Push to the Branch (`git push origin feature/YourFeature`)
5. Open a Pull Request

## License
Distributed under the MIT License. See `LICENSE` for more information.

