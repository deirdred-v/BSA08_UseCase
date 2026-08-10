# Use Cases

Summary:
Use cases, a common way of describing requirements for systems that contain models of software system behavior or ways for users to interact with the system.

## Contents

1. [Chapter I](#chapter-i) \
   1.1. [Task 1. Haircut Appointment](#41) \
   1.2. [Task 2. Delivery of Orders](#42) \
   1.3. [Task 3. Warehouse Storage](#43)
2. [Chapter II](#chapter-ii) \
   2.1. [Exercise 00 — Description of Use Cases](#51) \
   2.2. [Exercise 01 — Description of Use Case Flows](#52) \
   2.3. [Exercise 02 — Description of Use Cases](#53) \
   2.4. [Exercise 03 — Description of Use Case Flows](#54) \
   2.5. [Exercise 04 — Description of Use Cases](#55) \
   2.6. [Exercise 05 — Description of Use Case Flows](#56)

## Chapter I <div id="chapter-i"></div>

### Description of tasks

### Task 1. Haircut Appointment <div id="41"></div>

The management of a chain of barbershops decided to implement an online booking system. The main objective is to develop the business by expanding the customer base through the possibility of online registration, as well as to reduce employee labour costs and manual labour by automatically informing customers through communication channels. 

Both registered and unregistered visitors can book an appointment on the website. When making an appointment, they can select the type of service: hairdressing or cosmetology, as well as the service itself, the master and the time from the available intervals. The system should provide automatic sending of reminders to clients through the communication channel chosen by the client (Telegram, WhatsApp, VK, SMS) according to the schedule set by the manager. After receiving a service, the system offers the client to evaluate the service and write suggestions on how to improve the work.

The schedule of masters and the services provided by each master should be entered by the manager, who may be more than one person. This person is also responsible for keeping the schedule up to date and adjusting it if necessary, communicating with customers manually, marking the service, charging and accepting payment, sending the payment data to the accounting department. The manager can also receive reports on completed services and view customer feedback.

Each master has the ability to view the schedule and appointments for their services, as well as customer reviews. 

### Task 2. Delivery of Orders <div id="42"></div>

During the lockdown, many grocery stores and food companies dramatically increased their online sales and the need for quick delivery of small quantities to individual customers increased. 

A group of students got together and decided to create a delivery service startup. The idea is to quickly receive information about orders, pickup location and time, delivery location, desired delivery dates, and distribute this information to couriers who will pick up the order at the pickup location and deliver it to the delivery location. They decided to develop an online system where orders could be collected and quickly sorted for delivery by couriers.

The first step was to collect orders from stores and caterers in any way possible and have the operator enter them into the system in a consistent format, as well as developing a mobile application for the courier. The courier should be able to view order information, select an order from those available, book it, pick it up at the collection point and deliver it to the customer. The result of the courier's actions should be immediately reflected in the system via a mobile application. The system should also include a dispatcher who controls the couriers and reassigns orders if necessary. Information on received orders should be sent to the accounting department (to another IT system) to calculate delivery charges with order suppliers. Order delivery information should also be sent to the accounting department to calculate payment to couriers. Accrued payment should be transferred to the system and displayed in the courier's personal account. And there should also be an administrator's workstation, where couriers are registered and access rights are assigned to all of them.

### Task 3. Warehouse Storage <div id="43"></div>

A logistics company engaged in cargo transportation has decided to expand its business and organize the lease of warehouses for temporary or permanent storage of things and goods for individuals and legal entities. It is planned to rent and build warehouses in different parts of the city. The first: "Kamorka" — a system in the company, which provides accounting of rent of individual boxes of size from 3 to 15 square meters by individuals for storage of personal belongings, furniture, sports equipment.

The management of the company (customer) decided to introduce a centralized rental accounting of boxes, occupied and vacant, payment, access control and cleaning after vacating. Access to the warehouse itself is provided by a third party security company, which needs to be informed about new or dropped customers. The security company issues an electronic pass to the storage area for the specified period of time, extends or stops the validity of the pass in case of renewal or early termination of the lease agreement. The boxes are cleaned by the cleaning company after their use and before they are handed over to a new client. The purpose of the system implementation is to reduce manual work and personnel costs, reduce overhead costs, optimize box filling (minimize idle time of empty boxes), operational accounting of cash flow.

The client (individual) contacts the logistics company and through the manager concludes a contract for renting a box of the required size. To do this, the manager must have up-to-date information about available and soon-to-be vacant boxes. The client does not interact directly with the system, all information is provided by the manager. When the contract expires, the manager warns the client of the need to renew or terminate the contract and vacate the box. The manager is also responsible for organizing the cleaning of the boxes by a third-party company after they are vacated, as well as for organizing the client's access to the storage area, which is provided by a security company. After signing the contract, the manager informs the storekeeper about the allocation of a particular vacant box. The storekeeper checks the availability of the box (release of the previous tenant's belongings and cleaning), hands over the key to the box to the client, controls the release and cleaning of the boxes.

The team has an accountant. He/she calculates payments and controls income, payments to clients, payments for cleaning of boxes and security of the warehouse. The accountant receives information about new contracts and their changes from the manager. The payment for the cleaning of the boxes is calculated monthly on the basis of the area, the payment for the security — also monthly on the basis of the number of clients of the logistics company.

## Chapter II <div id="chapter-ii"></div>

### Exercise 00 — Description of Use Cases <div id="51"></div>

For Task 1, use the Use Case form to describe the interaction with the system to ensure that the system contains the actual schedule of master services without taking into account occupied and free slots. 

1. Apply the conditions of the task. In case of uncertainty, it is acceptable to add an additional condition by specifying it in the "Assumptions" section.
2. Identify the main actor whose business goal the system is supposed to solve in the use case and who is the initiator of the interaction with the system. 
3. Describe the purpose of the use case: the business need of the main actor, the business goal to be solved by the system using the use case.  
4. Provide a unique identifier for the use case.
5. Provide the name of the use case, a short unique title that describes the main action or purpose of the action in the format: <verb> + <noun> + <complement>. 
6. Identify the role of the Actor interacting with the system within the use case and their interest (need).
7. Identify at least 2 other stakeholders for whom the outcome of the use case is important. Identify their interests.
8. Specify the precondition of the use case: one or more conditions that must be true before the use case is executed. If there is no precondition, specify its absence.
9. Specify the use case trigger: the event that triggers the use case (action, temporary event, state change).
10. Specify the postconditions (conditions that must be true when the use case is completed):
    1. minimal guarantees: conditions that must be true at each end of the use case;
    2. success guarantees: conditions that must be true when a use case succeeds. 
11. Indicate your answers in the file `ex00_<product prefix>_US.docx`.

### Exercise 01 — Description of Use Case Flows <div id="52"></div>

For Task 1, use the Use Case form to describe the functional interaction for providing the actual schedule of master services in the system (without taking into account occupied and free slots) (Use Case described in ex.00).

1. When describing flows, use simple short sentences in the format: <*stakeholder or system*> <action to be performed> <conditions and/or constraints> *(subject — predicate — complements)*.
2. Use business rather than technical terms to describe steps.
3. All data transferred in a single time interval from a single source in a single direction should be transferred in a single step. 
4. Maintain the use case level in all its description up to the 5th level of nesting or implement an extension — another use case.
5. Minimize branching: use "The system confirms..." instead of "The system checks...". (To avoid writing "If... then...").
6. Reduce complex interactions to e.g. 4 transaction steps:
   1. The stakeholder enters the request, transfers the data;
   2. The system confirms the correctness of the input;
   3. The system modifies ....;
   4. The system outputs the result ...
7. If there are additional materials (user interface descriptions, prototypes, business rules, etc.) — place them separately from the use case, specify them with a link in the Additional field.
8. Describe the main scenario of the use case, using a numerical numbering of steps.
9. Number alternative scenarios with letters in relation to the step of the main scenario.
10. Alternate scenario steps should be numbered with:
    1. the step number of the main scenario;
    2. the letter of the branch from the main scenario step (alternate scenario letter);
    3. the step number within the alternate scenario.
11. Indicate your answers in the file `ex01_<product prefix>_US.docx`.

### Exercise 02 — Description of Use Cases <div id="53"></div>

For Task 1, use the Use Case form to describe how the client interacts with the system to select master services and book the selected slots.

1. Describe the use cases as required in 1-11 ex.00.
Identify one or more separate use case(s) with an "include" or "extend" relationship.  
3. Specify the type of relationship for each identified use case.
4. Indicate your answers in the file e`x02_<product prefix>_US.docx`.

### Exercise 03 — Description of Use Case Flows <div id="54"></div>

For Task 1, describe the basic flow and alternative flows of functional interaction between the client and the system to select a service and book a slot. 

1. Describe the flows of the use case(s) as required in 1-11 ex.01.
2. Describe the flows of the identified use case(s).  
3. Indicate your answers in the file `ex03_<product prefix>_US.docx`.

### Exercise 04 — Description of Use Cases <div id="55"></div>

For Task 1, use the Use Case form to describe the Master's interaction with the system in terms of viewing clients' booked services, their schedules, and clients' feedback on the work. 

1. Describe the use cases as required in 1-11 ex.00.
2. Identify a separate use case(s), with an "include" or "extend" relationship. 
3. Specify the type of relationship for each identified use case.
4. Indicate your answers in the file `ex04_<product prefix>_US.docx`.

### Exercise 05 — Description of Use Case Flows <div id="56"></div>

For Task 1, describe the basic flow and alternative flows of functional interaction between the master and the system to view services booked by clients and client feedback on the work. 

1. Describe the flows of the use case(s) as required in 1-11 ex.01.
2. Describe the flows of the identified use case(s). 
3. Indicate your answers in the file `ex05_<product prefix>_US.docx`.
