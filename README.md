# Introduction

How to check availability of whatever in programming language and database ?

# The problem

The problem i want to solve here should be work with different use cases, for example:

### Case 1: Car Rental

An user want to rent a car, but he want to know if the car is available in the date he want to rent.

Business rules:

- The car can be rented for a minimum of 7 days.
- The pickup hour must be between 8:00 and 18:00 (business hours).
- The return date must be at least 1 hour greater than the pickup date.
- Car can happen to be damaged, so the car can be unavailable for a period of time.

### Case 2: Room Reservation

An user want to reserve a room, but he want to know if the room is available in the date he want to reserve.

Business rules:

- The room must be reserved for a minimum of 1 night.
- The check-in date must be greater than the current date.
- The check-out date must be at least 1 day greater than the check-in date.
- The check-in hour must be after 14:00
- The check-out hour must be before 12:00
- The cleaning time is from 12:00 to 14:00
- Something can be destroyed in the room, so the room can be unavailable for a period of time.

### Case 3: Renting bikes

An user want to rent a bike, but he want to know if the bike is available in the date he want to rent.

Business rules:

- The bike can be rented for minimum of 15 minutes.
- All rental should have a idle time ( it will dependes on the bike type ).
- The bike can be damaged, so the bike can be unavailable for a period of time.


# Considerations

- Whatever language/framework/tests/etc you want.
- You can use any database you want.

# API

- Should get many items availability at once in a period of time.
- Should get one item availability in a period of time.

