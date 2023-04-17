
## Requirements
*The system must be able to:*
- Add an employee
- Remove an employee
- Pay each employee (after a set amount of time, say 2 weeks)
- Keep track of each employee's hours worked and adjust pay appropriately

### Design Patterns Used
- Observer Pattern
	- Paying all employees at the end of a pay period
- Singleton Pattern 
	- There can only exist a single instance of the EmployeeManager class


## Classes
### Employee Class
**Derives From:** None
*Attributes:*
- *string* name
- *uint* ID
- *float* payRate = 13.50

*Methods:*
- clock_in() -> *void*
- clock_out() -> *void*
- get_name() -> *string*
- get_ID() -> *uint*
- get_payRate() -> *float*

#### Cashier Class
**Derives From:** Employee
*Attributes:*

*Methods:*

#### Waiter Class
**Derives From:** Employee
*Attributes:*

*Methods:*

#### Line Cook Class
**Derives From:** Employee
*Attributes:*

*Methods:*

#### Manager Class
**Derives From:** Employee
*Attributes:*
- *float* payRate = $15

*Methods:*
- hireEmployee(*Employee* newEmployee) -> *void*
- fireEmployee(*Employee* targetEmployee) -> *void*


### Employee Manager Class
**Derives From:** None
*Attributes:*
- *vector\<Employee\>*  employeeRoster
- *float* currentPayPeriodTotal
- 

*Methods:*
- payout_all() -> void
- reset_pay_period() -> void
- get_employees(*String* : occupation = None) -> *vector\<Employee>\*
- 