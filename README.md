##AirBnB clone - The console

An Airbnb clone console project typically involves creating a command-line interface (CLI) that mimics some functionalities of Airbnb. The command interpreter serves as the interface through which users can interact with the system. It allows users to perform various operations like managing listings, users, bookings, etc., similar to how one might interact with Airbnb's platform.

# Description of the Command Interpreter:

#Starting the Console:
To start the Airbnb clone console, initiate it by running a Python script that launches the command line interface. 
python console.py 

#Using the Console:
Once the console is running, users can interact by typing commands and providing arguments to perform different actions. Here are examples of commands and their usage:

#Managing Listings:
create_listing <parameters>: Creates a new property listing with details like location, price, description, etc.
update_listing <listing_id> <parameters>: Updates an existing listing with new information.
delete_listing <listing_id>: Removes a listing from the system.

#Managing Users:
create_user <username> <email> <password>: Registers a new user in the system.
update_user <user_id> <parameters>: Modifies user information such as email, password, etc.
delete_user <user_id>: Deletes a user account.

#Handling Bookings:

** make_booking <user_id> <listing_id> <dates>: Allows a user to book a property for specified dates.
** cancel_booking <booking_id>: Cancels a previously made booking.
** view_bookings <user_id>: Displays all bookings made by a specific user.

#Examples:

Creating a Listing:
	create_listing "New York Apartment" --location "New York City" --price 150 --description "Cozy apartment in Manhattan" 

Updating a User's Email:
	update_user 1234 --email newemail@example.com 

Making a Booking:
	make_booking 5678 9876 "2023-12-20" "2023-12-25"

These examples illustrate how a user might interact with the Airbnb clone console by entering commands and providing necessary arguments to perform various operations related to listings, users, and bookings.

#Execution
Code works like this in interactive mode:

$ ./console.py
(hbnb) help

Documented commands (type help <topic>):
========================================
EOF  help  quit

(hbnb) 
(hbnb) 
(hbnb) quit
$

Code works like this in non- interactive mode:
$ echo "help" | ./console.py
(hbnb)

Documented commands (type help <topic>):
========================================
EOF  help  quit
(hbnb) 
$
$ cat test_help
help
$
$ cat test_help | ./console.py
(hbnb)

Documented commands (type help <topic>):
========================================
EOF  help  quit
(hbnb) 
$

Thanks
