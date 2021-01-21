# Rent-A-Ride
 Database Implementation for Car Rental Application

### Project Overview:
This project is basically to create a database for an application named “Rent-A-Ride” that allows users to rent a car based on car’s make and model.   
Generally, people look out for a temporary car when they do not own a car, or when visiting different cities/countries, or people who are waiting for their car to be repaired in order to get ease for their travel.This application allows a customer to select a car based on different car categories like SUV, Mini-Van, Sedan etc. Also, it provides a flexibility to customers to select the car based on different locations from where he can pick-up and return the car based on his ease and comfort.  
Here is the basic functionality of my application. This application is used by customers who would like to rent a car.   
Customer first download the App or visits the website and registers himself. He will then be provided a list of cars available to rent based on his choices of car’s category and location. He then selects a car and reserves it providing the date and timeframe for which he would like to rent. Customers who don’t have a vehicle’s insurance are required to take the rental insurance plan or if they already have an insurance, they have the flexibility to buy the rental plan or not. Apart from these customers are charged a late-fee, if they return the car after the due-date. If the customer takes the membership, he will be provided a default membership discount of 10% in addition to several discount offers offered by my system. 
  
### Entities:
1.	Customer
2.	Member
3.	Non-Member
4.	Car
5.	Car Category
6.	Location
7.	Booking
8.	Discount
9.	Rental Insurance
10.	Invoice
11.	Billing  
   
### Rent-A-Ride Structural Rules:
1.	Each car belongs to a particular category. Each category will have several cars.  
2.	A customer can be a member or a non-member of the application.  
3.	Each car is associated to a location. Each location can have single or multiple cars.  
4.	Each customer has one or multiple bookings. Each booking is associated to one customer.  
5.	A customer can have many invoices related to a booking. Each booking can have many invoices but all of them are related to a single customer only.  
6.	Each booking is related with only one car at a time. Each car may have none or at-most one booking (a single booking is allowed for a particular car and this car can’t be allotted to other customer unless and until the first customer cancels his booking).  
7.	Each booking has a pickup/drop-off location. Each location can have different bookings for pick-up and drop-off the cars.  
8.	Each booking can have at-most one discount. Each discount code can be applied to multiple bookings.  
9.	Each booking may have a rental insurance. A rental insurance may be associated to multiple bookings.  
10.	A single bill is generated for multiple invoices associated with a particular booking. A single bill is generated for a customer when he returns the car.    

### Conceptual ERD:
![Conceptual](https://user-images.githubusercontent.com/60439971/105414441-7e63e580-5c05-11eb-8607-82af1fd6fb89.png)

### Physical ERD:
![Physical-Physical jpg-Physical](https://user-images.githubusercontent.com/60439971/105414515-96d40000-5c05-11eb-8981-9b02ef402c51.png)

