# Little Lemon Web Application

## Introduction 
This is the final project for Meta Back-End Developer Capstone course (https://www.coursera.org/learn/back-end-developer-capstone/)

This web application utilizes Django + DRF + djoser + MySql.  
There is a simple static page with URL: http://localhost:8000/restaurant/

## APIs

### `restaurant/api/menu`
- Allows all authenticated users to view the menu items.  
- Only admin users can post new items.

**Fields needed to post:**
- **title**: str  
- **price**: decimal  
- **featured**: (optional) boolean, default = 0  

---

### `restaurant/api/menu/<int:pk>`
- Allows all authenticated users to view a single menu item.  
- Only admin users can update or delete a single item.  

---

### `restaurant/api/book`
- Allows authenticated users to post a new booking (use the same username of the user as the booking name).  
- Users can obtain all the bookings that have the same booking name as their username.

**Fields needed to post:**
- **name**: str (same as username)  
- **guest_number**: (optional) int, default = 1  
- **date**: date, in the form of "YYYY-MM-DD"  
- **comment**: (optional) text  

---

### `restaurant/api/book/<int:pk>`
- Only admin users can view or delete a single booking.  

---

## Current Users

### Superuser/Admin:
- **Username**: admin  
- **Password**: 123  

### Customers:
- **Username**: customer1  
- **Password**: lemon@123!  

- **Username**: customer2  
- **Password**: lemon@123!  
