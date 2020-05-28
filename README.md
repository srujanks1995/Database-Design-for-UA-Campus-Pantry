# Database Design for Campus Pantry

Language: PL/SQL, ASP.Net, HTML, CSS, Javascript, D3.js
Database: Oracle database
Cloud tools: Microsoft Azure 

#Requirements Analysis

UA Campus Pantry (UACP) is a nonprofit organization at the University of Arizona that provides
free food to college students in low-income households during the school year.
Three times a week, students can come to one Pantry to pick up items. UACP has student
profiles that record the student’s unique ID, first name, last name, date of birth, an email, an
address, and a contact number. Students will bring their bags to a checkout, where order details
are recorded. UACP keeps track of the order date-time stamp, quantity (which is recorded as
total pounds), and estimated cost, which is calculated by multiplying the weight by $1.52.
UACP purchases products from vendors. For vendors, UACP records a unique ID, name, an
address, a description, an email, and a contact number. Products are identified by a unique
product ID, which is associated with more details about a product, including name, description,
estimated cost, and weight. Products can be either be produce or nonperishables. For produce,
they record the estimated length of time until it will expire. For nonperishables, they record if it is
gluten-free. With each purchase, specific information about the order is recorded. This includes
date/time stamp of purchase, the quantity of a product purchased, cost per item, and calculate
the total cost by multiplying quantity by item cost.
Purchased products are converted to weight and details of the date time and weight quantity are
stored. These weighted products are added to a warehouse stock (there can be many
warehouses), along with additional warehouse details like quantity stored and date time stamp.
The warehouse stock is used to stock a warehouse, where details like ID, name, email,
address, description, and contact number are recorded for each warehouse. When stock in a
warehouse expires, it is recorded in a wasted table that keeps track of the date/time when the
food was wasted, the quantity (which is recorded as a weight), and the estimated cost is
calculated by multiplying the quantity by $1.52.
UACP will occasionally donate items from a warehouse to various organizations. In these
donation details, they record date/time, the total donated weight, and the number of bags
donated. For organizations, they keep track of the organization's ID, name, description, contact
number, email, and address.

A pantry will receive its items from a warehouse. For pantries, they record a pantry ID, name,
contact number, address, email, and description. To track when items move from a warehouse
to a pantry, transaction details are recorded. This includes transaction ID, weight, description,
and date/time stamp. A shift team handles each transaction and can handle many transactions
overall. Shift teams have a team ID and date/time stamp and will also include the start and end
time of the shift. A shift team is made up of staff, Chairs, and Volunteers. They record a focus
area for chairs and graduation dates for volunteers. A shift team can have up to one Chair and
up to three volunteers. Chairs and volunteers can be in more than one shift team. There are
three other types of staff, coordinator, student director, and graduate assistants. For a
coordinator, they record degree obtained, for the student director they record the year in school,
and for graduate assistants, they record if training is over. A staff member can only be one staff
type. For staff members, they record id, date of birth, address, username, password, contact
number, first name, last name, email address, start date, weekly distribution hours, end date,
and weekly operating hours.
Finally, donors make donations to the pantry. They keep track of donor details, including ID,
name, contact number, address, description, and email. For all donations, they keep track of a
donation ID, gift type, and date/time stamp. Donations can be either in-kind or money. For
in-kind, they record the weight of donation, food description, and calculate the monetary value of
the food donation by multiplying the weight by $1.52. For monetary donations, they record the
monetary amount. Food donations are added to the warehouse stock.


![](slides/Slide4.JPG)
![](slides/Slide5.JPG)
![](slides/Slide6.JPG)
![](slides/Slide7.JPG)
![](slides/Slide8.JPG)
![](slides/Slide9.JPG)
![](slides/Slide10.JPG)
![](slides/Slide11.JPG)
![](slides/Slide12.JPG)
![](slides/Slide13.JPG)
![](slides/Slide14.JPG)
![](slides/Slide15.JPG)
![](slides/Slide16.JPG)
![](slides/Slide17.JPG)
![](slides/Slide18.JPG)

