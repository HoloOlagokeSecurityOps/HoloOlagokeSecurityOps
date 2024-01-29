# Google Cybersecurity Professional - SQL Queries Filter in Linux OS

## Table of contents

- [Overview](#overview)
  - [The objective](#the-objective)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Tools used](#tools-used)
  - [Achievement](#achievement)
- [Author](#author)

## Overview



### The objective

- Screenshots of queries or typed versions of the queries

- Explanations of queries

- A project description at the beginning

- A summary at the end

- Details on using LIKE to search for a pattern

- Details on filtering for dates and times

- Details on using AND and OR to filter on multiple conditions

- Details on using NOT in filters

### Screenshot

![Retrieve failed login attempt](./Image/Retrieve%20fail%20login%20attempts%20after%20work%20hour.png)

![Retrieve login attempt on specific date](./Image/Check%20login%20attempt%20between%20dates%20A.png)

![Retrieve login outside mexico](./Image/Check%20login%20attempt%20not%20from%20Mexico%20A.png)

![Retrieve employee in marketing](./Image/Check%20staff%20from%20Marketing%20department.png)

![Retrieve employee in finacial or sales](./Image/Check%20staff%20from%20Finance%20or%20Sales%20department%20A.png)

![Retrieve employee not in IT](./Image/Check%20staff%20not%20from%20IT%20department%20A.png)

### Links

[Document link]

- [Apply filter to SQL Queries](https://docs.google.com/document/d/1zi7Hpj_sc_XxOjngXCr4dnBOKLQQ3wLWNR7dd2vfK94/edit?usp=drive_link)

## My process

To retrieve failed login attempt, I used the following commands

```sql

SELECT * /* select all columns */
FROM log_in_attempts /* log_in_attempts table */
WHERE login_time > "18:00:00" AND source = 0 /* where login time is grater than 6pm and attempt was not successful */
;

```

To retrieve login attempt on specific date, I used the following commands

```sql

SELECT * /* select all columns */
FROM log_in_attempts /* log_in_attempts table */
WHERE login_date = '2022-05-08' OR login_date = '2022-05-09' /* where login date is 8th May, 2022 or 9th May, 2022 */
;

```
To retrieve login attempt outside Mexico, I used the following commands

```sql

SELECT * /* select all columns */
FROM log_in_attempts /* log_in_attempts table */
WHERE NOT country LIKE 'Mex%' /* where country column does not start with the word "Mex"  */
;

```

To retrieve employee from marketing department, I used the following commands

```sql

SELECT * /* select all columns */
FROM employee /* employee table */
WHERE department = 'marketing' AND office LIKE 'East%' /* where department column is "marketing" and office column start with the word "East"  */
;

```

To retrieve employee from finance or sales department, I used the following commands

```sql

SELECT * /* select all columns */
FROM employee /* employee table */
WHERE department = 'finance' OR department = 'sales' /* where department is either "finance" or "sales"  */
;

```

To retrieve employee not in IT department, I used the following commands

```sql

SELECT * /* select all columns */
FROM employee /* employee table */
WHERE NOT department = 'IT' /* where department is not from "IT" */
;

```

### Tools Used

- Linux OS
- Bash
- mySQL

### Achievement

- Investigate failed login attempt after work hours

- Investigate suspicious login attempt on specific date

- Retrieve login attempt outside Mexico country

- Retrieve employees data from different department

## Author

[LinkedIn](www.linkedin.com/in/olagoke-holo)

[Facebook](https://web.facebook.com/olagoke.holo.3/)

[Twitter](https://twitter.com/olarragoken)

[Instagram](https://www.instagram.com/holoolagoke/)
