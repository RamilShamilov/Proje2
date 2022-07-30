# Proje2
#Chapter 2 ##Object-oriented programming

Your department receives a request to prepare a test software to digitalize the health insurance, logistics, and trading companies that can be expanded in the future.

You come up with an idea: object-oriented programming. Your approach is to create classes for each company that will have different attributes and methods to digitalize some of their functions.

Health insurance
Define the class
You start with the health insurance company.

You need to create a system for the supplemental health insurance registration process by taking different variables like age, chronic disease, and income into account.

📌 Use the keyword "class" to create the class "HealthInsurance"

📌 Use the "init" method to initialze the object's attributes: self, company_name, foundation_year, founder_name, company_slogan, num_of_employees and num_of_clients.

Define the methods
Next, define the methods of the class:

print_report method: A method to print out information about the company.

📌 The report should have this structure:

"The company name, was founded in year. The founder of the company is founder_name.

Company slogan: company_slogan

Number of employees: number of employees

Number of clients: number of clients"

sup_health_insurance method: A method to check the eligibility for supplemental health insurance. It should consider the parameters "age", "chronic_disease", and "income".

📌 Use if-else statements and logical operators.

update_num_clients method: A method to update the attribute number of clients.

#Define the "HealthInsurance" class
class healthinsurance:
    #Initialize the object's attributes
    def __init__(self, company_name, foundation_year, founder_name, company_slogan, num_of-employee, num_of_clients)
    self.company_name = company_name
    self.foundation_year = foundation_year
    self.founder_name = founder_name
    self.company_slogan = company_slogan
    self.num_of_employees = num_of_employees
    self.num_of_clients = num_of_clients
    
​
​
    #Define the print_report method
    def print_report(self):
        print(f"""The company{self.company_name} was founded in {self.foundation_year}.
        The founder of the company is {self.founder_name}.
        Company slogan: {self.company_slogan}
        number of employee: {self.num_of_employees}
        Number of clients: {self.num_of_clients}""")
​
    #Define the sup_health_insurance method
    def sup_health_insurancce(self, age, chronic_disease, income):
      #if-else statements to check whether person can get supplemental insurance or not
      if age >= 60 and chronic _disease == True and income < 6000:
            print("We are sorry! You are not eligible for supplemental health insurance.")
    elif age < 60 and income >= 6000 or chronic_disease  == False:
            print("Congratulations! You can get supplemental health insurance.")
​
    #Define the update_num_clients method
    def update_sum_clients(self, new_number):
        self.num_of_clients = new_number 
        print(f"Number of clients has been changed to {self.num_of_clients}!")
​
  Input In [1]
    def __init__(self, company_name, foundation_year, founder_name, company_slogan, num_of-employee, num_of_clients)
                                                                                          ^
SyntaxError: invalid syntax


Create the object
Now that we created our class and initialized its attributes and methods, we can create the object “HI_company1” with the attributes:

Company_name “Healthy”

foundation_year “2012”

founder_name “Bob Mayer”

company_slogan “We care for you.”

num_of_employees “3500”

num_of_clients “13230”

#Create the object "HI_company1" with it's attributes
HI_company1 = Healthinsurance('Healthy', 2012, 'Bob Mayer', We care for you.)
  Input In [2]
    HI_company1 = Healthinsurance('Healthy', 2012, 'Bob Mayer', We care for you.)
                                                                   ^
SyntaxError: invalid syntax


Let’s check if the methods work.
There is a new customer that wants to register for supplemental health insurance. He is 45 years old, does not have a chronic disease, and has an income of 5000 dollars per month.

📌 Use the sup_health_insurance method with this information.

#Use the sup_health_insurance for the new customer
HI_company1.suphealth_insurance_(45, False, 5000)
---------------------------------------------------------------------------
NameError                                 Traceback (most recent call last)
Input In [3], in <cell line: 2>()
      1 #Use the sup_health_insurance for the new customer
----> 2 HI_company1.suphealth_insurance_(45, False, 5000)

NameError: name 'HI_company1' is not defined

Because the number of clients has increased, you should use the update_num_clients method.

📌 The new_number will be 13231.

#Update the number of clients
HI_company1.update_num_clients(13231)
---------------------------------------------------------------------------
NameError                                 Traceback (most recent call last)
Input In [4], in <cell line: 2>()
      1 #Update the number of clients
----> 2 HI_company1.update_num_clients(13231)

NameError: name 'HI_company1' is not defined

To see the output of the latest update and check whether it worked or not, call the print_report method.

#Call the print_report method for HI_company1
HI_company1.print__report()
---------------------------------------------------------------------------
NameError                                 Traceback (most recent call last)
Input In [5], in <cell line: 2>()
      1 #Call the print_report method for HI_company1
----> 2 HI_company1.print__report()

NameError: name 'HI_company1' is not defined

Logistic
Let's continue with the next company from your brief.

Storage plays a crucial part in logistics, and the company wants to track the status of inventory space with software and be able to make changes in the system whenever it is needed.

Again, you need to create a class.

📌 Use the keyword "class" to create the class "Logistics"

📌 Use the "init" method to initialze the object's attributes: self, company_name, foundation_year, founder_name, company_slogan, and inventory_space.

Define the methods
Next, define the methods of the class:

print_report method: A method to print out information about the company.

📌 The report should have this structure:

"The company name, was founded in year. The founder of the company is founder_name.

Company slogan: company_slogan

Inventory space of the company: inventory_space

update_inventory_space method: A method to update its inventory_space, and print a statement to describe the change. It should consider the parameter "new_storage_space".
#Define the "Logistics" class
class Logistics
    #Initialize the object's attributes 
    def __init__(self, company_name, foundation_year, founder_name, company-slogan, inventory_space):
        self.company_nsme = company_name
        self.foundation_year = foundation_year
        self_company_slogan = company_slogan
        self.inventory_space = inventory_space
    
    
        
    #Define the print_report method
    def print_report(self):
        print(f"""
        The company name is {self.company_name} and was founded in {self.foundation_year}.
        The founder of the company is {self.founder_name}.
        Comppany_slogan: {self.company_sllogan}
        INventory space of the company: {self.inventory_space}""")
    
​
    #Define the update_inventory_space method
    
def update_inventory_space(self, new_storage_space):
    self.inventory_space = new_storage_space
    print(f"Inventory space has been changed to {self.inventory_space}!")
​
  Input In [6]
    class Logistics
                   ^
SyntaxError: invalid syntax


Create the object
Now that we created our class and initialized its attributes and methods, we can create the object “logistic_company1” with the attributes:

Company_name “LogCom”

foundation_year “1990”

founder_name “Laura McCartey”

company_slogan “There is no place we cannot reach.”

inventory_space “2500”

#Create the object "logistic_company1" with it's attributes
logistic_company1 = logistic("LogCom", 1990, "Laura McCartey", "There is no place we cannot reach.", 2500)
---------------------------------------------------------------------------
NameError                                 Traceback (most recent call last)
Input In [8], in <cell line: 2>()
      1 #Create the object "logistic_company1" with it's attributes
----> 2 logistic_company1 = logistic("LogCom", 1990, "Laura McCartey", "There is no place we cannot reach.", 2500)

NameError: name 'logistic' is not defined

Let’s check if the methods work.
The logistics company plans to buy a new warehouse which will increase the inventory_space to 3000.

📌 Call the update_inventory_space method to reflect this change in the system and then use the “print_report” method.

#Update the inventory space
logistic_company1.update_inventory_space(3000)
#Call the print_report method for logistic_company1
logistic_company1.print_report()
Trading
The last company you need to digitalize is the trading one.

You are expected to create a method to update the sales and expenses and calculate the revenue.

As with the previous companies, you need to create a class.

📌 Use the keyword "class" to create the class "Trading"

📌 Use the "init" method to initialze the object's attributes: self, company_name, foundation_year, founder_name, company_slogan, sales, expenses, and revenue.

Define the methods
Next, define the methods of the class:

print_report method: A method to print out information about the company.

📌 The report should have this structure:

"The company name, was founded in year. The founder of the company is founder_name.

Company slogan: company_slogan

Total sales: sales

Total expenses: expenses

Total revenue: revenue

update_sales_and_expenses method: A method to update the sales and expenses. It should consider the parameters "new_sales" and "new_expenses".

calculate_revenue method: A method which computes the difference between sales and expenses and prints out the revenue.

#Define the "Trading" class
class Trading:
    #Initialize the object's attributes 
    def __init__(self, company_name, foundation_name, founde_name, company_slogan, sales, expenses, revenue):
        self.compnay_name = company_name 
        self.foundation_year = foundation_year
        self.founder_name = founder_name
        self.company_slogan = company_slogan
        self.revenue = revenue
        
​
    #Define the print_report method
    def print_report(self):
        print(f"""
        The company name is {self.company_name} and was founded in {self.foundation_year}. 
        The founder of the company is {self.founder_name}.
        Company slogan: {self.company_slogan}
        Toyal sales : {self.sales}
        Total expenses: {self.expenses}
        Total revenue: {self.revenue}""")
​
    #Define the update_sales_and_expenses method
    def update_sales_and_expenses(self, new_sales, new_expenses):
        self.sales += new_sales
        self.expenses += new_expenses
        print("Sales and expenses are updated!")
​
    #Define the calculate_revenue method
    def calculate_revenue(self):
        self.revenue = self.sales = self.expenses
        print(f"The revenue of the company is: {self.revenue}")
Create the object
Now that we created our class and initialized its attributes and methods, we can create the object “trading_company1” with the attributes:

Company_name “TraCom”

foundation_year “2005”

founder_name “Chong Wu”

company_slogan “We revolutionize trading.”

sales "5000"

expenses "2000"

revenue "3000"

#Create the object "trading_company1" with it's attributes
trading_company1 = Trading('TraCom', 2005, 'Chong Wu', 'We revelutionize tarding.', 5000, 2000, 3000)
Let’s check if the methods work.
Update the sales and expenses. The sales went up by 100 and the expenses increased by 50.

📌 Use the update_sales_and_expenses method with this information.

#Update the sales and expenses
trading_company1.update_sales_and_expenses(100, 50)
---------------------------------------------------------------------------
NameError                                 Traceback (most recent call last)
Input In [9], in <cell line: 2>()
      1 #Update the sales and expenses
----> 2 trading_company1.update_sales_and_expenses(100, 50)

NameError: name 'trading_company1' is not defined

After updating sale and expense informations, it is time to calculate the company revenue.

📌 Use the calculate revenue method.

#Calculate the revenue
trading.company1.calculate_revenue()
Finally, let’s check our company’s information.

#Call the print_report method for trading_company1
trading_company1.print_report()
---------------------------------------------------------------------------
NameError                                 Traceback (most recent call last)
Input In [11], in <cell line: 2>()
      1 #Call the print_report method for trading_company1
----> 2 trading_company1.print_report()

NameError: name 'trading_company1' is not defined
