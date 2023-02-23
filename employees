SELECT * FROM employees;

SELECT id, name, job_id, department_id, salary, sh_clerk, commission_pct, phone_num FROM employees WHERE name = 'David';

SELECT id from employees WHERE sh_clerk = 'Manager';

SELECT * FROM employees WHERE first_name LIKE '%a%a%';

SELECT * FROM employees WHERE first_name LIKE '%l' AND LENGTH (first_name) > 5;

SELECT ROUND ((salary * 1.2) ,2) , '$' FROM employees;

SELECT '$', ROUND (salary + (salary * commission_pct / 100), 2) FROM employees;

SELECT employee.first_name, COUNT(*), manager.first_name 
FROM employees AS employee
INNER JOIN employees AS manager ON manager.manager_id = employees.manager_id
GROUP BY manager.first_name
HAVING COUNT(*) > 6;

SELECT department.deparment_name FROM department
JOIN employees ON department.department_id = employees.department_id
GROUP BY department.deparment_name
HAVING COUNT(*) > 30;

SELECT * FROM employees
WHERE salary > (SELECT AVG(Salary) FROM employees);

SELECT departments.department_name FROM departments
LEFT JOIN employees ON departments.department_id = employees.department_id
WHERE employees.employee_id IS NULL;













