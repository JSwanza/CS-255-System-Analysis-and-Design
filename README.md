# CS-255-System-Analysis-and-Design

This repository contains my work for SNHU's CS 255 course, including the Business Requirements Document (Project One) and System Design Document (Project Two) for the DriverPass project, along with this reflection.

## DriverPass Project Reflection

### Briefly summarize the DriverPass project. Who was the client? What type of system did they want you to design?

The DriverPass project was the main focus of CS 255. The client was DriverPass, a company that provides driver training to help people pass their DMV driving tests. They wanted a comprehensive web-based system to fix the problem of high failure rates (over 65% in some cases) due to poor preparation. The system needed to let customers register, buy training packages (with online classes, practice tests, and on-road lessons), schedule/modify/cancel two-hour driving sessions, track progress, view driver notes, and handle payments securely. It also required admin features for staff (secretaries, IT officers, owner) to manage users, reservations, reports, and DMV rule updates, all accessible online from any device with cloud hosting.

### What did you do particularly well?

I think I did a solid job capturing the client's needs directly from the interview transcript and turning them into clear, structured requirements. In the Business Requirements Document, I used "The system shall..." statements for functional requirements that matched exactly what DriverPass asked for—like the three packages, reservation matching to drivers/cars, activity logging, and offline report exports. For the System Design Document, I specified realistic technical details (cloud servers, PostgreSQL/MySQL, React frontend, security with 2FA/RBAC/HTTPS, performance for 1000 concurrent users under 2 seconds) and included UML diagrams created in Lucidchart. My bulleted format made everything easy to reference when moving from requirements to design.


(Examples of use case diagrams similar to what I created, showing actors like Customer, Administrator, Secretary, and use cases for login, scheduling, reporting, etc.)

### If you could choose one part of your work on these documents to revise, what would you pick? How would you improve it?

I'd revise the UML diagrams section in the System Design Document. While I included the diagrams (use case, activity, sequence, class), I could have added more detailed descriptions or annotations for each one—explaining key actors, flows, relationships, and how they tie back to specific requirements. For example, explicitly noting include/extend relationships in the use case or error handling in sequence diagrams would make them clearer for anyone reviewing the portfolio later. I'd also ensure the class diagram shows more attributes/methods for core entities like Reservation, Package, User, and Car/Driver.


(Example class diagrams for vehicle/driver/reservation systems—mine was similar but tailored to DriverPass with classes like Customer, Reservation, Package, Driver, Car.)

### How did you interpret the user’s needs and implement them into your system design? Why is it so important to consider the user’s needs when designing?

I interpreted DriverPass's needs by going line-by-line through the interview transcript—things like multiple user roles, package options, scheduling logistics with 10 cars/drivers, DMV integration notifications, secure payments, and printable/exportable reports—and mapped them straight into "shall" statements and technical specs. For instance, role-based access (customers only see their data, admins have full control) came directly from their security concerns, and cloud accessibility addressed "any device" access. Considering user needs is critical because it ensures the system actually solves their problems, gets adopted, avoids wasted development on unused features, and prevents costly changes later. If you ignore stakeholders, you build something that doesn't fit real-world use.

### How do you approach designing software? What techniques or strategies would you use in the future to analyze and design a system?

My approach starts with gathering and analyzing requirements (stakeholder interviews, use cases), then modeling with UML (use case/activity/sequence/class diagrams), defining nonfunctional aspects early (security, performance, scalability), and documenting everything clearly. For the DriverPass project, Lucidchart for diagrams, bulleted requirements, and referencing the transcript worked well. In the future, I'd add more iterative feedback (maybe quick prototypes or user stories), use MoSCoW prioritization for features, and incorporate agile practices like sprints even in coursework. I'd also do early risk assessments (e.g., cloud downtime, payment gateway integration) and validate UI sketches with potential users.


(Example Gantt chart—mine showed phases like requirements gathering, UML diagramming, technical design, and review aligned with the interview timeline.)

Overall, this project strengthened my skills in translating business needs into technical designs. I'm proud of how closely my documents followed DriverPass's vision!
