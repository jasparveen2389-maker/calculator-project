Hostel/Flat Expense Splitter
This is a simple Python program that helps you calculate the monthly amount each person needs to pay in a shared hostel room or flat.
It divides the total expenses—rent, food, and electricity equally among all residents.

Features:
Takes user input for:
Rent of the hostel/flat
Total food ordered
Electricity units consumed
Charge per electricity unit
Number of persons sharing the room/flat


Calculates:
Total electricity bill
Combined monthly expenditure
Amount each person has to pay
Provides a clean and simple output.

Input Required:
The program will ask for the following:
1. Hostel/Flat Rent
2. Total Food Ordered (₹)
3. Electricity Units Spent
4. Charge Per Unit (₹)
5. Number of People Living Together

How the Calculation Works
1. Calculate electricity bill:
total_bill = electricity_spend * charge_per_unit

2. Add all expenses:
total_expenses = rent + food + total_bill

3. Divide by total persons:
each_person_pays = total_expenses // persons

Code:
rent = int(input("Enter your hostel/flat rent: "))
food = int(input("Enter the amount of food ordered: "))
electricity_spend = int(input("Enter the total electricity spend: "))
charge_per_unit = int(input("Enter the charge per unit: "))
persons = int(input("Enter the number of persons living in room/flat: "))

total_bill = electricity_spend * charge_per_unit
output = (food + rent + total_bill) // persons
print("Each person will pay = ", output)

Output Example
Enter your hostel/flat rent: 8000
Enter the amount of food ordered: 3000
Enter the total electricity spend: 120
Enter the charge per unit: 8
Enter the number of persons living in room/flat: 2

Each person will pay =  5720


Notes
Integer division (//) is used to avoid decimal values.
Change // to / if you want exact decimal amounts.
