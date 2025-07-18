# Agile Model and Jira



* Agile Model - It is a model that contains some steps, using those steps we can develop the software to customer.
* Agile Model follows all the steps that are present in SDLC.
* Agile model was invented to solve the problems of waterfall model.



#### Waterfall Model follows SDLC.

1. Requirements Gathering
2. Feasibility Study
3. Design
4. Coding
5. Testing
6. Deployment
7. Maintenance



Waterfall model follows some rules:-

1. Companies should use waterfall model , if there are no new requirements given by the customer in the future, i.e all requirements should be available in the beginning itself.
2. Customer is not satisfied.
3. Requirements are freeze.
4. Development is fast.



#### Agile Model (Iterative + Incremental) -

change in requirements  is allowed by customer

customer satisfaction is achieved

3 ways available in it :

1. Scrum Methodology
2. Kanban
3. Xtreme Programming



Scrum Methodology :

1. Product Owner - responsible for collecting requirements from customer, P.O after collecting requirements is going to prepare User Stories, and split user stories in Epics.
2. Scrum Master - Head of scrum team, Conducts Meetings, tracking progress, solution to problems.
3. Scrum Team - Developers and Testers who work on project



1. **Customer** :

Develop a software similar to Gmail.

Login should happen and after than should be redirected to Inbox page

I want a search bar to search for the mails

I Want a feature that should send a message to mail id of a person as well as mobile no of a person

Logout feature should be there to logout from the application.



2\. **Product Owner**

He collects all those requirements above and understand it well

After understanding the requirements well he will prepare user stories



USER STORIES - They are features / functionalities that customer is expecting that should be developed to customer which is written in English sentence according to customers' perspective.

Ex. - Login should happen and after than should be redirected to Inbox page -> LOGIN FUNCTIONALITY



US-01

As a customer, I want to login using correct username and correct password

US-02

As a customer, I want that error message should be displayed while incorrect username and password.

US-03

As a customer, I want to login using correct username and correct password and navigate to Home Page.



These user stories are divided into smaller parts called as Tasks.



US-01

As a customer, I want to login using correct username and correct password



-> Login page should be developed

-> It should contain username and email and mobile no and password.

-> It should have a login button

-> Username should be accept max 256 characters



Diagram :



                                                                                                                                                                                                                  Daily Scrum/Standup Meeting (15 min)

                                                              																			  what you did today?, any problems are you facing?

                                                      																					what will you do tomorrow?

                                                                                                                                                                                                                                                |

                                                                                                                                                                                                                                                |

Customer --> Requirements ---> Product backlog(Word Document) ----------> Sprint Backlog ----------> Scrum Team  ===> 1 week to 5 week

                                                                                                                             Sprint                                                                                                     |

                                                                                                                      Planning Meeting                                                                                      |  -----> Sprint Review Meeting

                                                                                                                                                                                                                                             V

                                                                                                                                                                                                                                          Demonstration to customer





1. **Product Backlog** = It is a document all the USER STORIES written by product owner.
2. **Spring Backlog** = decided USER STORIES that is a part of this Sprint by Scrum Master.
3. **Sprint Planning Meeting** = SCRUM master conducts meeting with scrum team to decide which user stories can be a part of this sprint.
4. **Sprint** = It is a timeframe/ duration during which set of user stories will be developed and tested.
5. **Daily Standup Meeting** = This is a meeting conducted by scrum master with scrum team and 3 questions are asked 1) what you did today? 2) Any problems are you facing? 3) What will you do tomorrow?
6. **Sprint Review Meeting** = Customer will look at the part of the software developed and is going to give a feedback, he also confirms whether he want this software currently or after some sprints.
7. **Sprint Retrospect Meeting** = PO, SM and ST will analyze what went wrong and what went correct.



NOTE : Agile Model is Iterative and Incremental

Incremental - Every sprint makes the s/w to have more feature

Iterative - Same process gets repeated again and again until all the user stories are ready to the customer.





8\.   **Story Points**:

For every user story created by P.O team members (Dev, Testers, Architects, UI/UX Designer) give number to each user story - > story points



            Priority

US-01 ....  High

US-02 .... Medium



              |

              | sprint planning meeting

              |

              V



Sprint Backlog



            Priority   Story Point

US-01 ....  High       13

US-02 .... Medium   3



Priority - Importance

Story Point - Complexity



Story point is a number that basically tells how much complex (more tasks) a user story is



Fibonacci series = 1,1,2,3,5,8,....



What problems we get if we don't have story points?

1. Time calculation(sprint) will be difficult
2. Leads to confusion



Planning Poker: used to decide story points

Scrum Team -> 5 People -> 3 dev and 2 Testers and Designer



9\.  **Burndown Chart:** display the amount of work done in each day based on story points.



10\. **Velocity** : average value of the story points across various sprints that is basically uses as a reference for the upcoming sprints.



Note: Product Backlog (50 U.S) -> Sprint Backlog (15 U.S) -> Sprint (3 weeks) => Completed (12 U.S) then the remaining 3 will get added to Product Backlog again.



Issues in JIRA:

Issues in JIRA can be a EPIC or USER STORY or TASK or SUB-TASK



Requirements :

1. I want a login and a signup page
2. I want a feature to send a message to mail id
3. I want feature to search particular mail



EPIC - gives high level req.



Write down the EPIC's (Functionality) by looking at the requirements

* Login
* Signup
* New mail
* Search





write down the user stories for each and every epic:

**Login** 

US-01 -> As a customer, I want to login with valid username and email and password and redirect to homepage

US-02 -> As a customer, I want to display error message with invalid username/email and password

US-03 -> As a customer, I want the login button should be disable if username and password is not entered.



write down **Acceptance Criteria** for each and every user story:

Acceptance Criteria -> It is al list of check points that should be satisfied if we want to call a USER story is completed or not.



US-01 -> As a customer, I want to login with valid username and email and password and redirect to homepage



Acceptance Criteria for US-01:

1. Login Page should be ready
2. Enter valid credentials
3. Click on Login
4. Redirection to Home Page



Divide each user story into small parts and those small parts are called as **TASKs**



US-01: As a customer, I want to login with valid username and email and password and redirect to homepage.



* *Task 1* => Develop login page with username, password, and Login Button.
* *Task 2* => Test login page



Divide each TASK into even more smaller tasks called as **SUB-TASKs**



Task 1 => Develop login page with username, password and login button

* *SubTask 1* => Create a login UI using HTML
* *SubTask 2* => Apply CSS to that Login UI



Task 2 => Test login Page

* *SubTask 1* => Checking for valid credentials 
* *SubTask 2* => Checking for invalid credentials





Add the user stories to the Sprint Backlog 

Start the sprint (1 weeks to 5 weeks)



### JIRA



**Product Owner** create Epic and User Stories

Scrum Team(developer) create Tasks



Epic is parent of user story, in description write description

user story is parent of task, in description write acceptance criteria



Now handed over  to **Scrum master**

in backlog option;

put story and its tasks under it

do a meeting and then pull user stories and task from backlog to sprint

start a sprint

user story and task will appear in to do

first dev will push user story in progress and then task 

dev will work on task and then push in done, 

then testers will push their stories , in progress, then done

then finally user story will be done and finish!!





