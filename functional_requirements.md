# Functional Requirements for Car Rental System

### 1. Reservation System for Cars
- **Requirement**: The system should allow drivers to reserve a car (sedan, SUV, pickup, or van) at least 24 hours before the intended checkout time.
- **Black-box Test Case**:
  - **Test Input**: A driver attempts to make a reservation for a sedan at 3:00 PM on September 25 for checkout on September 24, 2:00 PM.
  - **Expected Output**: The system rejects the reservation, as it doesn't meet the 24-hour advance booking rule.

### 2. Reservation Extension
- **Requirement**: The system should allow drivers to request an extension for the return time, which can only be granted if no other reservation exists for the car.
- **Black-box Test Case**:
  - **Test Input**: A driver requests an extension for a car that is due at 5:00 PM, but another reservation exists for the same car at 6:00 PM.
  - **Expected Output**: The system denies the extension request and informs the driver about the conflict.

### 3. Different Rental Charges Based on Car Type
- **Requirement**: The system should calculate rental charges based on the type of car rented (e.g., sedans, SUVs, pickups, or vans), with different rates for each.
- **Black-box Test Case**:
  - **Test Input**: A driver rents a sedan for one day and an SUV for two days.
  - **Expected Output**: The system correctly calculates charges based on the rental durations and vehicle types, ensuring different rates are applied.

### 4. Discount for Long-Term Rentals
- **Requirement**: The system should apply a discount to rentals that last a week or longer.
- **Black-box Test Case**:
  - **Test Input**: A driver rents a car for 7 days.
  - **Expected Output**: The system applies the appropriate discount for long-term rentals.

### 5. Updating Rental Charges
- **Requirement**: The system should allow an admin or authorized user to update the rental charges for different types of cars.
- **Black-box Test Case**:
  - **Test Input**: An admin updates the rental charge for SUVs from $50/day to $60/day.
  - **Expected Output**: The system updates the rate successfully, and new reservations reflect the updated charge.
