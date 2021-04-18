# ⚕️ Hospital Management System - Made using C#, ASP.net

A fully featured Clinic Management System having a well designed Database Schema made as a final project for the course "Application Development with .NET and Web Services CS624" during my Semester at [Pace University](https://www.pace.edu/). Its based on the 3 Tier Architecture.

### Signup Page 
<img src="images/main1.png"/>

### Take Appointment
<img src="images/appointment1.png"/> 

### Current Appointments
<img src="images/current1.png"/> 

### Search Staff
<img src="images/search.png"/> 

### 1. Patient:

* **1.	Patient Home** – Patient can view his profile
* **2.	Current Appointment** – Patient can view if he has some pending or approved appointment with a doctor 
* **3.	Bills History** – Patient can view the bill history of appointments that have been completed
* **4.	Treatment History** – Patient can view the treatment history of appointments which have been completed
* **5.	Take Appointment** – Patient can view all the departments, and then can select one dept. Then the doctors of that dept are shown. Then patient selects one doctor and the doctor’s profile is then shown along with a ‘take appointment’ button. When the button is clicked, the free slots of that particular doctor are shown. Patient selects a free slot of his choice and then sends request for that free slot to the doctor. The doctor will then approve/reject it.
* **6.	Notifications** – In this tab, a notification is shown whenever the doctor accepts/rejects the requested appointment.
* **7.	Feedback** – After a appointment is completed, patient can give feedback about that appointment by rating it from 1 – 5
* **8.**	A patient can request for only one appointment at a time and will not be allowed to take more than one appointments until the last appointment has been completed.

### 2. Doctor:

* **1.	DoctorProfile**: Doctor can see his own profile
* **2.	PendingAppointments**: Doctor can see all the pending appointments against his doctor ID.
* **3.	TodaysAppointmemts**: the appointments for current day will be shown.The doctor then can select/reject any appointment of that day
* **4.	HistoryUpdate**: He can update prescription,disease and progress of patient 
* **5.	GenerateBill**: He will then generate the bill
* **6.	PatientHistory**: Doctor will be able to see the treatment history of all his treated patients. 

### 3. Administrator:

* **1. Admin Home**: Admin can view Clinic stats which includes weekly appointments, income of the Clinic. No of registered patients and doctors along with the list of departments 
* **2.	View Doctors**: Admin can view the list of doctors currently registered along with their departments and other information. Complete profile will be shown when clicked.
* **3.	View Patients**: Admin can view the list of patients currently registered along with their phone numbers and ids. Complete profile will be shown when clicked.
* **4.	View Other Staff**: Admin can view other staff members along with their designations.
* **5.	Search Box**: Admin can search for a specific employ within the company by name
* **6.	Add/Remove**: Admin can Add/remove doctors patients and other staff members form the clinic.


## How to Run
1- Install the following:
* [Microsoft Visual Studio](https://visualstudio.microsoft.com/vs/community/)
* [Microsoft SQL Server Express](https://www.microsoft.com/en-us/sql-server/sql-server-editions-express)
* [Microsoft SQL Server Management Studio (SSMS)](https://docs.microsoft.com/en-us/sql/ssms/download-sql-server-management-studio-ssms?view=sql-server-2017)

2- Open SQL Server Management Studio and in the "Connect to Database Engine" window type the following:
```
Servername: .\SQLEXRPESS
Authentication: Windows Authentication 
```
<p align="center">
<img src="images/connection.png" width = "500"/> 
</p>

3- Now open Schema.sql file in Database Files folder and execute it all. This will create the database and the tables. Afterwards execute the following sql files: Admin.sql, Doctor.sql, Patient.sql, Signup.sql.

4- Now execute the Insertions.sql file in Database Files folder. This will populate the database with some test entries. Moreover, some login emails and passwords of doctors, patients and admin are placed in the Insertions.sql file. You can use them to test the functionalities of the system.

5- Everything is setup now! You can run the Visual Studio Project by opening Clinic Management System.sln and then select the SignUp.aspx page and click run button named IIS Express. 
<p align="center">
<img src="images/run1.png"/> 
</p>
