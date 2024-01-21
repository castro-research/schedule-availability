# Introduction

How to check availability of whatever in programming language and database?

# The problem

The problem I want to solve here should be work with different use cases, for example:

### Case 1: Car Rental

An user wants to rent a car, but he wants to know if the car is available in the date he wants to rent.

Business rules:

- The car can be rented for a minimum of 7 days.
- The pickup hour must be between 8:00 and 18:00 (business hours).
- The return date must be at least 1 hour greater than the pickup date.
- Car can happen to be damaged, so the car can be unavailable for a period of time.

### Case 2: Room Reservation

An user want to reserve a room, but he want to know if the room is available in the date he wants to reserve.

Business rules:

- The room must be reserved for a minimum of 1 night.
- The check-in date must be greater than the current date.
- The check-out date must be at least 1 day greater than the check-in date.
- The check-in hour must be after 14:00
- The check-out hour must be before 12:00
- The cleaning time is from 12:00 to 14:00
- Something can be destroyed in the room, so the room can be unavailable for a period of time.

### Case 3: Renting bikes

An user wants to rent a bike, but he wants to know if the bike is available in the date he wants to rent.

Business rules:

- The bike can be rented for minimum of 15 minutes.
- All rental should have a idle time (it will dependes on the bike type).
- The bike can be rented for a maximum of 24 hours.
- It can be possible to check the availability of a bike grouped by bike type.
- The bike can be damaged, so the bike can be unavailable for a period of time.
- The bike damaged can be replaced by another same SKU bike if available.
- If bike is not available, it must show similar bikes available.
- By having others rental place, it must show a nearby place with available bikes. 

### Case 4: Tickets Availability

An user wants to buy a ticket, but he wants to know if the ticket is available in the date he wants to buy.

Business rules:

- The ticket can be bought an hour before the event.
- The ticket can be redeemedat any time.
- If the ticket is not available, it must show how many people got an interest in the ticket and receive a notification that it was unavaiable too. (How many people got an interest in the ticket).
- The user can ingress in a waiting list to receive a notification when the ticket is available.
- It must show how many places were avaiable.

### Case 5: Doctor appointment

An user wants to schedule a doctor appointment, but he wants to know if the doctor is available in the date he wants to schedule.

Business rules:

- The doctor only works from 8:00 to 18:00.
- The doctor can have a lunch break from 12:00 to 14:00.
- The doctor has an break between each appointment of 10 minutes.
- The user can schedule an appointment with max duration of 2 hours.
- The user can schedule an appoiiintment with min duration of 30 minutes.
- The user can ingress in a waiting list in case of withdraw.
- An user can only have a schedule per month.

# Considerations

- Whatever language/framework/tests/etc you want.
- You can use any database you want.

# API

- Should get many items availability at once in a period of time.
- Should get one item availability in a period of time.

