# private-project
|ID| content |
| ---| ---|
|Tpye | USABILTY |
|User story| add new features (funding system) to the original phd application system|
|Extended Description| new features are used to manage phd students' funding, there are three different roles in this system, each of those has different permissions|
|Roles| **SuperUser**: <br>1. have complete access.<br>   2. create new student record,have access to a dashboard which shown the information of enrolled students from current and past years. <br>3. have access to all information of supervisors.<br> **Supervisor** <br> 1. enter comments such as interview reports <br> 2. do not have access to see information of other supervisors <br> **Admin** <br> 1. have access to the information of all other applicants and funding in the system.<br>  2. Admin's access to the information is not determined by SUPERUSER, it has full access in viewing candidates' information.<br>3. do not have access to the dashboard  |
|status of applicants| 1. Enrolled<br>2. Suspended<br>3. Completed|
|Requirements| 1. Students should have an attribute named ni stored in the database to indicate whether they have a scholarship. If they are self-funded, this value should be set to 0, otherwise it should be set to the amount of fund they got. <br>2. Supervisors can supervise a set of students, so every supervisor should also have an attribute in the database named ntot. Ntot is the sum of ni of all supervised students. If a student is supervised with another academic, ni/2 should be added instead of ni. <br>3. Every supervisor has an upper limit on the amount of funding named nmax, the system should highlight if some supervisors have ntot>nmax (but not forbid it as there are exceptions).<br> 4. Super users can manually specify scholarship types and the amount of different scholarships. for example, superusers can set different scholarship types, such as type 1-10,000 pounds and type 2-20,000 pounds. Meanwhile, the value of type 1 can be changed from 10,000 to 15,000 pounds, but the original 10,000 pounds should be remembered to ensure that the amount of scholarship of students who have entered into the database will not be modified.|
|Language Type and Frame| Python JavaScript Flask|
|Means of Verification| Code review, unit tests, use cases


|ID|content|
|---|---|
|Role|Superuser|
|Description|Superuser should be able to create a student record|
|Requirement|1. Create a new student record |
