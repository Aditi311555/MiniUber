# MiniUber


## Overview

This Java program is a mini-project that simulates an Uber-like transportation service. It allows users to:
- **Create an account and log in**.
- **Rent a vehicle** for in-city and intercity travel.
- **Calculate costs** based on distance and vehicle type.
- **Send a package** with specific guidelines and pricing.

## Features

### User Features
1. **Account Management**: 
   - Users can create an account and log in to access services.

2. **Book a Ride**:
   - **Rent a car** for in-city travel (Hatchback, Sedan, SUV).
   - **Intercity travel** to predefined cities (e.g., Mumbai, Nagpur, Nashik).
   - **Send a package** with specific constraints (e.g., weight must be under 5kg).

3. **Pricing**:
   - Pricing is calculated based on distance and vehicle type.
   - A 5% GST is added to the total cost.

4. **OTP Verification**:
   - Users must verify their booking with an OTP sent to their mobile number.

5. **Vehicle Number Assignment**:
   - A random vehicle number is assigned to each booking.

6. **Waiting Time Simulation**:
   - Simulates a 5-second waiting time before the vehicle arrives.

### Admin Features
- **Admin Access**:
   - View or modify user data (currently in a basic implementation stage).

## Classes and Structure

### Main Classes
1. **Data**:
   - Handles account creation, login, OTP verification, and date handling.

2. **Transport**:
   - Manages locations, destinations, and calculations for rides.

3. **B (Booking)**:
   - Extends Transport and implements specific booking and vehicle choice features.

### Pricing Calculations
- **In-city trips**:
   - Base fare + distance-based charge (multiplied by a fixed rate).
   - GST is added on top of the total cost.
- **Intercity trips**:
   - Similar calculation as in-city trips with higher base fare.

## Sample Usage

1. **Start the Application**:
   - Compile and run the program.
   - Choose between "User" and "Admin" access.

2. **User Flow**:
   - Create an account and log in.
   - Select a service (Rent a Car, Intercity Travel, or Send a Package).
   - Confirm booking details and OTP.
   - View total cost with GST and assigned vehicle number.

## Code Overview

### Important Methods
- **createAccount()**: Handles user account creation.
- **login()**: User login functionality.
- **destination()**: Accepts destination input for in-city rides.
- **intercityDestination()**: Accepts destination input for intercity rides.
- **otp()**: Simulates OTP verification.
- **waiting()**: Simulates vehicle arrival time.

### Example Input/Output

```
Enter
1.User
2.Admin
1

-----CREATE ACCOUNT-----
Enter username:
JohnDoe
Enter Password:
1234
ACCOUNT CREATED SUCCESSFULLY

-----LOGIN PAGE-----
Enter username:
JohnDoe
Enter Password:
1234
Logged in successfully!!

**********WELCOME TO UBER SERVICES**********
ENTER YOUR CHOICE NUMBER
1. Rent a car
2. Intercity
3. Trip
4. Send a package
```

## Requirements

- **Java Development Kit (JDK)** 11 or higher.
- **Java IDE** like Eclipse or IntelliJ IDEA for editing and running the code.

## Installation

1. **Download the Code**:
   - Clone the repository or download the zip file.

2. **Compile the Program**:
   - Open a terminal or command prompt.
   - Navigate to the project directory and run:
     ```
     javac mini/uber.java
     ```

3. **Run the Program**:
   ```
   java mini.uber
   ```


## License

This project is open-source and free to use. 

---

Feel free to update any sections as per your requirements or add more details if needed.
