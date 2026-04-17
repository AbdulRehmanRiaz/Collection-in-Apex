# Collection-in-Apex
Generic implementation of APEX Collections demonstrating temporary data handling with add, update, delete, and final save to database including image support and validations

**APEX Collection – Generic Implementation**
This project demonstrates the working of APEX Collections in Oracle APEX using a generic employee form. <br>

It shows how to:

Temporarily store data in collections <br>
Perform Add, Update, Delete operations <br>
Handle image data <br>
Finally save data into database table <br>

**What is APEX Collection?**

APEX Collection is a session-based temporary storage used to hold data before committing it to database.<br>

Works like a cart system <br>
Data remains until session ends or collection is deleted <br>

<img src="images/collection%20home.png" width="700"/> <br>

<img src="images/collection%20backend%20page.png" width="700"/>

**Application Flow**

1️⃣ **Employee Form (Data Entry)**
A form is created to capture:<br>
Employee Name <br>
Job <br>
Salary <br>
Image <br>

<img src="images/collection%20form.png" width="700"/>

2️⃣ **Add to Collection**
Data entered in form is added to collection <br>
Uses APEX_COLLECTION.ADD_MEMBER <br>
add to colelction query is added to code folder in this repositry <br>

<img src="images/add%20collection.png" width="700"/>


3️⃣ **Collection Report (View Data)**
Displays all collection data<br>
Includes: <br>
Name<br>
Job<br>
Salary<br>
Image<br>

<img src="images/collection%20report.png" width="700"/>

4️⃣ Update Collection Member<br>
Each row has an Update button<br>
Uses SEQ_ID to identify record<br>
Updates collection using UPDATE_MEMBER<br>
update colelction query is added to code folder in this repositry<br>

<img src="images/collection%20edit%20form%20and%20report.png" width="700"/><br>
<img src="images/collection%20update%20dynamic%20action.png" width="700"/>
<img src="images/update%20collection.png" width="700"/>


5️⃣ Delete Collection Member
Delete button removes record from collection<br>
Uses SEQ_ID<br>
delete colelction query is added to code folder in this repositry<br>

<img src="images/collection%20delete.png" width="700"/><br>
<img src="images/collection%20delete%20dynamic%20action.png" width="700"/>
<img src="images/delete%20collection.png" width="700"/>


6️⃣ Save Data to Table
All collection records are inserted into database table<br>
Collection is cleared after save<br>
save to table query is added to code folder in this repositry<br>

<img src="images/save%20collection%20data%20to%20table.png" width="700"/>


7️⃣ Final Table Report
Displays saved data from database<br>
Image is also viewable<br>

<img src="images/emp%20table%20report.png" width="700"/>


8️⃣ Validations
Implemented NOT NULL validations on:<br>
Employee Name<br>
Job<br>
Salary<br>
<img src="images/collection%20validations%20and%20processes.png" width="700"/>

