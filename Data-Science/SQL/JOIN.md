2024-09-29 15:22

Status:

Tags:
[[SQL]]

# JOIN

#### INNER JOIN

	SELECT username, operating_system, employees.device_id
	FROM  employees
	INNER JOIN machines ON employees.device_id = machines.device_id;

This is used to join two or more tables in order to get a query from them for example, in the query above we are querying operating_system and employees.device_id from employees and we are joining the tables machines & employees using device_id that appears in both.

also in this case since username and operating_system don't appear in both they can be used normally but in the case of device_id since it does appear in both we must specify which ones to return by specifying both the table and the column name: employees.device_id / machines.device_id

#### OUTER JOIN

This command expands what is returned from joining two or more tables, each type of outerjoin returns all rows from either one table or both tables.

#### LEFT JOIN

	SELECT *
	FROM employees
	LEFT JOIN machines ON employees.device_id = machines.device_id;

 In this example we are joining the machine table into employees query telling it to just bring only records that match the right table machines, thus the `employees.device_id = machines.device_id` we are joining the right into the left. 

#### RIGHT JOIN

	SELECT *
	FROM employees
	RIGHT JOIN machines ON employees.device_id = machines.device_id;

Right join has the same syntax as `LEFT JOIN` but it produces a different output, since its inversed, in this case it would return the exact same result.

#### FULL OUTER JOINS

Returns all records from both tables. you could think of it as merging them.

	SELECT *
	FROM employees
	FULL OUTER JOIN machines ON employees.device_id = machines.device_id;

the result of this query would be all records from both tables, similar to `INNER JOIN` the order of the tables does no change the result of the query.


References 