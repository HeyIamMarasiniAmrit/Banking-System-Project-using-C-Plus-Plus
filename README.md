# Banking-System-Project-using-C-Plus-Plus
It is a project for banking providing the minimal features of the banking system. We can perform the following tasks in this project.  
1.Create an Account
2.Check Balance in a particular Account
3.Deposit or withdraw cash from a particular Account
4.Close any particular Account
5.List all the Accounts

Working Procedure of Banking System Project using C++:
In this project, we have written some classes for different purposes and the main function. We have taken a constant MIN_BALANCE of value 500. Then we have a class InsufficientFunds which will act as an exception for insufficient funds.

Next, we created a class Account. This class is having accountNumber, firstName, lastName, balance, and NextAccountNumber (of type static). If you want more details then you can add more variables. Then we have defined the default constructor and parameterized constructor for class Account. Then we have some getters or accessors i.e. getAccNo (), getFirstName () etc. We haven’t written mutators because all these things cannot be modified. Once the account number is assigned it cannot be changed. And the first name and last name of a person cannot be changed associated with that account.

Next, we have defined functions for deposit and withdrawal. Then for accessing the static member that is NextAccountNumber, we have created two static functions that are setLastAccountNumber () and getLastAccountNumber (). We are using files for storing the data. If we quit the program then we will start again then Account should know what was the last account number and what should be the next account number.

Then for saving in the file and retrieving from the file, we have created friend functions. Also, to display the details of the Account, we have an overloaded insertion operator which is ostream operator.

Next, we created a class Bank. Bank will have a collection of Accounts so we have created an object accounts of type map. Because we are searching based on the account number so we have taken a map. The first type of map is the account number and the second is the Account class itself. This map container is useful for storing all the accounts. So when the program starts it should get all the account details from the file and store them.

So, when we will be using the application then the application will be accessing the columns. Then we have defined all the necessary functions for this class and some functions we have defined outside the class.
