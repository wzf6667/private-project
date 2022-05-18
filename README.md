# private-project
|ID| content |
| ---| ---|
|Tpye | USABILTY |
|User story| add new features (funding system) to the original phd application system|
|Roles| SuperUser: <br>1. have complete access.<br>   2. create new student record,have access to a dashboard which shown the information of enrolled students from current and past years. <br>3. have access to all information of supervisors|
|Requirements| 1. Students should have an attribute named ni stored in the database to indicate whether they have a scholarship. If they are self-funded, this value should be set to 0, otherwise it should be set to the amount of fund they got. |
| |2. Supervisors can supervise a set of students, so every supervisor should also have an attribute in the database named ntot. Ntot is the sum of ni of all supervised students. If a student is supervised with another academic, ni/2 should be added instead of ni. |
| |3. Every supervisor has an upper limit on the amount of funding named nmax, the system should highlight if some supervisors have ntot>nmax (but not forbid it as there are exceptions). |
| |4. Super users can manually specify scholarship types and the amount of different scholarships. for example, superusers can set different scholarship types, such as type 1-10,000 pounds and type 2-20,000 pounds. Meanwhile, the value of type 1 can be changed from 10,000 to 15,000 pounds, but the original 10,000 pounds should be remembered to ensure that the amount of scholarship of students who have entered into the database will not be modified.|
