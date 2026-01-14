# Functional Requirements
## Movie Management
- The system shall allow storing and managing movie information, including:
      - Name
      - Length
      - Release date
      - Directors
      - Distributors
      - Description (About)
      - List of genres
      - Ticket price
- The system shall maintain a list of available movies using a linked list.
- The system shall allow users to view all available movies.
- The system shall allow searching for movies by name and/or genre.

## Showtime Management
- The system shall store showtime information, including:
    - Associated movie
    - Start time
    - End time
    - Assigned cinema hall
- The system shall maintain available showtimes using an array.
- The system shall allow users to view showtimes for a selected movie.
- The system shall prevent scheduling two movies at the same time.
- The system shall associate each showtime with its own seat availability.
- The system shall clone or assign a cinema hall seat layout to each showtime to ensure seat independence between movies.

## Cinema Hall and Seat Management
- The system shall store cinema hall details, including:
    - Hall number
    - Array (2D) of seats
- The system shall maintain cinema halls using a HashMap, keyed by hall number.
- The system shall represent seats using row and column numbers.
- The system shall track seat availability per showtime.
- The system shall prevent double-booking of the same seat within the same showtime.
- The system shall allow users to select one or more seats per reservation.

## Ticket Reservation
- The system shall allow users to reserve tickets.
- The system shall allow a client to reserve multiple seats in a single reservation.
- The system shall collect reservation details including:
    - Client name
    - Contact information
    - Cinema hall number
    - List of selected seats
    - Date
    - Time
    - Movie name
    - Total price
- The system shall store ticket reservation requests in a queue, processed in order of receipt.
- The system shall allow seat reservation through:
    - Ticket
    - MovieShowtime
    - CinemaHall classes
- The system shall allow reservations to be canceled or modified using a stack structure.

## Payment Processing
- The system shall allow users to pay for tickets.
- The system shall support the following payment modes:
    - Cash
    - Debit
    - Credit
- The system shall calculate the total cost based on:
    - Ticket price
    - Number of seats
