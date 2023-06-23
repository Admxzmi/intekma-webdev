# **Calendar Management System Design**

## **Database Design**

### **Entity Relation Diagram**

![ERD](/sajesaje.drawio%20(3).png)

### **Realtionships**

- One department can have multiple events (one-to-many relationship).
- One event can be assigned to one department (one-to-one relationship).
- One department can have multiple subdivisions (one-to-many relationship).
- One event can be assigned to one subdivision (one-to-one relationship).

## **System Process Flow**

1. **User** logs into the Calendar management System.
2. The system retrieves the **user's**authorized **departments** and **subdivisions**.
3. **User** selects a **department** to view **events**.
4. The system fetches **events** associated with selected **department**, including **events** from all **subdivisions** within the **department**
5. **User** can further filter the **events** based on **subdivisions**.
6. System displays the filtered **events** to the **user**.
7. **User** can create, update, delete **events**.
8. For **event** creation/update, the **user** selects the **department** and **subdivision**, provides **event** details, and specifies the start and end dates/times.
9. The system validates the inputs, saves the **event*8 to the database, and updates the calendar view.
10. **User** can modify or delete existing **events**, and the system updates the database accordingly.
11. **User** can switch between **departments** or **subdivisions** to view **events** from different areas.
12. **User** can log out of the system, and the session ends.


The system design allows for efficient management of events based on departments and subdivisions, providing flexibility and scalability for an organization with unlimited levels of sub-subdivisions within each department.
