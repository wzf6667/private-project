# private-project



|ID|content|
|---|---|
|Role|Superuser|
|Description|Superuser should be able to **create** a student record|
|Requirement|1. Create a new student record |

|ID|content|
|---|---|
|Role|Superuser|
|Description|Superuser should be able to **Add** or **Modify** scholarship types|
|Requirement|1. add a new type of scholarship.<br> 2. modify an existing scholarship, at the meanwhile, the original data of this type should be reserved to ensure that the amount of the scholarship does not change for students who have received this type of scholarship in the past|

|ID|content|
|---|---|
|Role|Superuser|
|Description|Superuser should be able to **add supervisors** for phd students|
|Requirement|1. Add supervisor to a phd student.<br> 2. some students may have more than one supervisors |

|ID|content|
|---|---|
|Role|Superuser|
|Description|Superuser should be able to **allocate fundings** to **students**|
|Requirement|1. allocate one type of scholarship for a student.<br> 2. If the student is self-funded, the type of scholarship should be set to self-funded |

|ID|content|
|---|---|
|Role|Superuser|
|Description|Superuser should be able to **allocate fundings** for **supervisors**|
|Requirement|1. superuser should allocate fundings for each supervisor manually |


|ID|content|
|---|---|
|Role|Superuser|
|Description|Superuser should have access to a **dashboard**|
|Requirement|1. The dashboard should show the number of scholarships for all students (current and past) per supervisor, the total amount of scholarships for all students per supervisor|

|ID|content|
|---|---|
|Role|Superuser|
|Description|Superuser should be able to discover supervisors whose fund used in excess of allocated funds|
|Requirement|1. The system should highlight those supervisors in the dashboard.<br>2. This situation is not forbidden |

|ID|content|
|---|---|
|Role|Supervisor|
|Description|Supervisor should be able to read all related data|
|Requirement|1. Supervisors are able to read the scholarship amount and total for each student under supervision, as well as the amount of funds received from the school.<br>2. If a student is supervised jointly with another supervisor, half of the student's scholarship amount is provided by one supervisor.<br> 3. Supervisors can only read information of students who are under their supervision|

|ID|content|
|---|---|
|Role|Admin|
|Description|Admin should be able to read all information of students|
|Requirement|1.Admin is able to read students' information.<br> 2. They do not have access to the dashboard |

**ACTIONS**
1. as a superuser, I want to create a new student record 
2. as a superuser, I want to add a new scholarship type, if I want to overwrite the old scholarship type, I should keep the data of the old scholarship type 
3. as a superuser, I want to add a supervisor for a phd student 
4. as a superuser, I want to assign scholarship to the student, if no scholarships should be marked as 0 
5. as a superuser, I want to assign funds manually to supervisors 
6. as a superuser, I want to get a dashboard that shows the number of scholarships for all students (current and past) for each supervisor, the total amount of scholarships for all students 
7. as a superuser, I want the system to be able to highlight in the dashboard those supervisors whose remaining funding exceeds a threshold. 
8. As a supervisor, I want to be able to read the amount of scholarships and the total amount of scholarships for each student under my supervision, as well as the amount of funding I receive from the school. If a student is co-supervised with another supervisor, half of the student's scholarship amount is provided by myself 
9. As a supervisor, I can only view the information of the students I supervise 
10. As an admin, I want to be able to view the information of all students, but not access the dashboard

















