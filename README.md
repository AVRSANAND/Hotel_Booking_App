# Hotel Booking Project

This Python project allows users to see a list of hotels, book a hotel, and receive a reservation confirmation ticket. The app is implemented using Object-Oriented Programming (OOP) principles.

## Features

- **View Hotels**: Users can view a list of available hotels.
- **Book Hotels**: Users can book a hotel.
- **Credit Card**: Users provide their credit card details to book hotel. 
- **Reservation Confirmation**: Users receive a reservation confirmation ticket upon booking.

## Booking Process: 
Follow the prompts to enter the hotel ID and your name to book a hotel. If the hotel is available, it will be booked, and a reservation confirmation ticket will be generated.

## Files

- `main.py`: Main script to manage hotel bookings.
- `plan.txt`: Contains a brief plan and features of the app.
- `hotels.csv`: Data file containing hotel information (not provided here).
- `cards.csv`: Data file containing credit cards information. 

## Requirements

- `pandas`

You can install the required package using:

```bash
pip install pandas
```

## Usage
Prepare the Data: Ensure you have a hotels.csv file with the necessary hotel data. The CSV should have columns id, name, and available (with yes or no values for availability).

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/AVRSANAND/Hotel_Booking_App.git
    cd Hotel_Booking_App
    ```

2. Run the Script: Execute the following command to run the booking script:
    ```bash
    python main.py
    ```
    
## Classes

### Hotel

**Attributes:**

- `hotel_id`: ID of the hotel.
- `name`: Name of the hotel.

**Methods:**

- `book()`: Books the hotel by changing its availability to "no".
- `available()`: Checks if the hotel is available.

### ReservationTicket

**Attributes:**

- `customer_name`: Name of the customer.
- `hotel`: Hotel object associated with the reservation.

**Methods:**

- `generate()`: Generates a reservation confirmation ticket.

### CreditCard

**Attributes:**

- `number`: Credit Card number

**Methods**

- `validate()`: Validates the credit card information.

## Sample Data

Example entry in hotels.csv:

```
id,name,available
1,Hotel Sunshine,yes
2,Hotel Moonlight,no
3,Hotel Starlight,yes
```
Example entry in cards.csv:

```
number,expiration,cvv,holder
"1234567890123456","12/26","123","AVRS ANAND"
"5678901234567890","12/28","456","JOHN SMITH"
```
