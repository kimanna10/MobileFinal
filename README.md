# MobileFinal
Mobile Kim Anna IS1711 (23934)

# CoffeeMM
# Description: This app allows you to easily make an order without going to the bar, register, log in, view coffee and make an order, as well as change the composition of the desired coffee, respectively, to find out when his order is ready.
# Main Goal: The goal is to create an app that will reduce the time to order coffee and wait.
# Main Problem: The problem is time waiting for an order in a coffee shop and creating queues.
Language: Java
Platform: Android App
Functional: UseCase


# REGISTRATION
Actors: User, System
Goals: User-Register in the system; System-Add new user to DB
Scenario: 
1. User launches the system, then clicks on “Registration” button; The system opens session and offers to login or register, then opens registration window;
2. User fills all fields; System check for error(e.g password should consist 8 symbol etc) , then add user to DB
3. System show popup “You have been successfully registered”
Result: User has been successfully registered and may work with the system;
# LOGIN
Actors: User, System
Goals: User-Login to the system and start to work; System-identify user and permissions 
Scenario: 
1. User launches the system; The system opens session and offers to enter login and password;
2. User inputs the password and login; System check it;
3. System show popup “You have been successfully logged in”
Result: User has been successfully logged in and may work with the system
# ORDERING COFFEE
Actors: User, System
Goals: User-Order of coffee ; System-Add this request to DB
Scenario: 
1. User launches the system, presses on “Order” button , the finds right coffee; The system opens “Order” window;
2. User books current coffee; System checks the request, then add it to DB, if it not exists in DB( if this coffee is left)
Result: User has been successfully ordered the coffee
# VIEW/SEARCH COFFEE
 Actors: User, System
Goals: User-View/Search the coffee; System-Show all information from user’s request
Scenario: 
1. User launches the system, click on “Coffee” button; The system opens “Coffee” window;
2. User enter request; System check the request, then shows all information about user’s request, if it exists in DB
Result: User has been successfully view all or certain information about coffee
# CHANGING COFFEE CONTENT
Actors: User, System
Goals: User-change content of coffee; System-Add this request to DB
Scenario: 
1. User launches the system, presses on “Order” button , the finds right coffee; The system opens “Order” window;
2. User books current coffee and change it’s content; System checks the request, then add it to DB, if it not exists in DB( if this coffee topping is left)
Result: User has been successfully ordered the coffee
# LOG OUT
Actors: User, System
Goals: User-Logout; System-Ends the session 
Scenario: 
1. User pressed on “Log out” button; The system asks “Do you want to log out?”;
2. User pressed “yes”; System ends the session, logs out 
Result: User has been successfully logged out from the system


# Functional Requirements 
1. Authentication of user when he/she tries to login into system
2. System should to execute the request of Order and coffee booking
3. Search for coffee and pull them out of the DB
4. Change the coffee content if user wants
5. System should provide “Manage order of coffee”
6. End of session on logout
