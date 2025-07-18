# Security Testing:



##### Android O.S Problems:-

1\) No security for third-party apps

2\) Delay in software updates

3\) Pre-installed applications(Bloatware)



##### Various ways available to achieved security (Device/App) :

1\) Always download apps from verified sources (play store, Appstore)

2\) Give the permission to the app which is controlled by the user.

3\) Use some lock mechanism (PIN, Pattern, ...)

4\) Use Antivirus software

5\) **Security** by Masking data ( hide the data (WIFI name = capg\_01 => acceptable\_01))

6\) **Encryption** :

Password ==> BCRYPT ( hash()) ==> encrypted data

Salt are random character added to your encrypted data

7\) **XSS attack**( Cross Site Scripting) - It is a attack where the hacker will try to introduce some JavaScript code through the UI.

We have to sanitize(removing unwanted data) the incoming data( >, <, \*, !, - Ignore) => cloud ware

8\) **SQL Injection**: It is a attack where the attacker tries to modify the SQL query to trick the database.

insert into registration(username, password) values ( username, password)

                                                                                                    "1"=="1", "1"=="1"

select \* from registration where username = "1" == "1"

Sanitize

9\) **CSRF (Cross Site Request Forgery)** - When hacker tricks the logged-in user from original website into sending unauthorized commands.

CSRF token is set with every page and when user sends the data token is attached to it, and if server sees the data along with token it will accept it and if not it will reject.



###### There are some rules in which, a developer following those rules will make the application secure.

10 rules where developers will make mistake (given by OWASP(open worldwide application security project)):

1. **Broken Access Control:** There is some access/permission given to a person, the permission is broken. Example: /display?='Name' where name can be anything, url will display result of any person which should not happen, giving access to everyone. (Privilege issue).
2. Follow Encryption.
3. Handle Injections(SQL, XSS, ...) properly.
4. Develop with secure design. Example : Reset password with OTP, Banking application allows to change the password with OTP, application helps to change the old password to new password which is not same.
5. Still using the old components in the software.
6. **Broken Authentication**: Most developers, will create a login page that is weak, which can lead to an entry point for the hackers. Example: If a person is trying to login with wrong info more than 3 times, disable the login page / don't allow that login page to used by that person. using MFA/OTP
7. Don't use third party plugins/tools that are not verified.
8. Focus on monitoring the application. Example: 1000 requests sent within 1 hour from same Ip address but admin is not alert.
9. Handle Forgery (CSRF).

10\.

HTTP and HTTPS

VPN(Virtual Private Network)

HTTP----> VPN -----> Application





#### Test Environment Management (TEM):

* Environment that is dedicated for testing activities.



* Who will manage (setup) this environment? 

&nbsp;     ***Cloud Engineer, DEVOP's Engineer, Test Environment Engineer***



* What does this environment consist?

1. &nbsp;Server
2. Database



The data that is used to run the tests in test environment is Test data

Username = "Raju'

Password= "Welcome"



Note: The test case required for our application will be stored inside the database.



**Automation Testing:**

A tool executes the test cases, data is in MySQL DB.



Mockaroo generates the fake test data



Problems if we use these tools to generate data:

1. Duplicate data
2. Privacy issue and legal suit (mask the data \*\*\*\*2312)



How they will manage/set up the Test Environment?

1. Use Automation tool like TERRAFORM



&nbsp;      Config File -----> Terraform -----> AWS

&nbsp;      (provider, VPC, Internet Gateway, Instances, server specs)



2\.   Install the required tool like python, jdk, etc using ANSIBLE.



&nbsp;      requirements file -----> Ansible ------> Server 1

&nbsp;                                                          \\   \\\_\_\_\_ > Server 2

&nbsp;                                                            \\\_\_\_\_\_\_> Server 3



###### What are the challenges we face if there is poor TEM?

1. Delays in the project
2. Configuration issues / version issues
3. Difficult to monitor
4. Inconsistency(some tests pass and some fail)













