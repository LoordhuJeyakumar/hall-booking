# Hall Booking API

This API provides endpoints for managing room bookings, customers, and booking details and customer booking counts.

## **Links**

## [Render Deployed URL 👈](https://hall-booking-api-o14n.onrender.com)

`https://hall-booking-api-o14n.onrender.com`

## [Github repository URL 👈](https://github.com/LoordhuJeyakumar/hall-booking)

`https://github.com/LoordhuJeyakumar/hall-booking`

## [Postman documentation URL 👈](https://documenter.getpostman.com/view/27536086/2s9YsFEuE8)

`https://documenter.getpostman.com/view/27536086/2s9YsFEuE8`

## **Endpoints:**

- **<p style="color:#FFE460">POST</p> /api/v1/createRoom:**
  - **Description:** Creates a new room in the system.
  - **Request Body:** Room details (name, capacity, etc.)
  - **Response:** 201 Created with the new room details on success, or appropriate error response.
- **<span style="color:#FFE460">POST</span> /api/v1/booking:**
  - **Description:** Books a room for a customer.
  - **Request Body:** Booking details (customer information, room name, date, time, etc.)
  - **Response:** 201 Created with a success message on successful booking, or 404 Not Found if the room is not available, or other error responses.
- **<span style="color:#6BDD9A">GET</span> /api/v1/rooms:**
  - **Description:** Retrieves a list of all rooms in the system.
  - **Response:** 200 OK with an array of room details.
- **<span style="color:#6BDD9A">GET</span> /api/v1/customers:**
  - **Description:** Retrieves a list of all customers in the system.
  - **Response:** 200 OK with an array of customer details.
- **<span style="color:#6BDD9A">GET</span> /api/v1/bookingDetails:**
  - **Description:** Retrieves a list of all booking details in the system.
  - **Response:** 200 OK with an array of booking details.
- **<span style="color:#6BDD9A">GET</span> /api/v1/bookedRooms:**
  - **Description:** Retrieves a list of rooms that are currently booked.
  - **Response:** 200 OK with an array of booked room details, including booking confirmation IDs and related customer information.
- **<span style="color:#6BDD9A">GET</span> /api/v1/customerBookings:**
  - **Description:** Retrieves a list of bookings for a specific customer.
  - **Response:** 200 OK with an array of bookings for the customer, including booking details and total bookings.
- **<span style="color:#6BDD9A">GET</span> /api/v1/nonBookedRooms:**
  - **Description:** Retrieves a list of rooms that are currently not booked.
  - **Response:** 200 OK with an array of available room details.
