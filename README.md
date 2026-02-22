# Grazioso Salvare Database Application
## Professional Self-Assessment

In my Computer Science program, I dived into a bunch of different topics, and learned how to do all sorts of things. From DAD-220 (Intro to Struct. Database Env.), where I learned how to create and interact with databases, to CS-465 (Full-Stack Development I), where I observed and enacted the creation of a full-stack application. Classes like CS-250 (Software Development Lifecycle) taught me about utilizing the SDLC to keep a project on track, how to interact with people in different positions in a team environment, and how to keep shareholders in the loop throughout the process, while other classes like CS-305 (Software Security) taught me how to protect against common attacks such as SQL injection and impersonation. Even in the class I was taking in parallel to the capstone class (CS-370: Current/Emerging Trends in CS) I learned how to create artificially intelligent algorithms capable of learning over time. In the constantly changing environments of the various classes where I frequently had to learn the basics of unfamiliar programming languages in a very short period, I learned how to be flexible and adapt to new circumstances. 

For my capstone project, rather than making small changes to a few small projects, I decided to expand one small project into a significantly larger project in terms of how much I created. It started with a small, messy project from CS-340 (Client/Server Development), which consisted of a single page that showed database entries from a MongoDB database, generated a pie chart and map based on table data, and allowed the user to do some very basic search operations on the table, such as applying some preset filters (with somewhat ambiguous names) or searching single values. It also included a simple CRUD (Create, Read, Update, and Delete) module for interacting with the database, although the application only ever read from the database. First, with the understanding that I developed from CS-250 (that you’re writing software for other people who might not know everything you do), I decided to create helper buttons next to the filter options to give exact definitions of what each of the various filters do. This was both to prove that I can make more accessible software, and that I could communicate ideas clearly within an application. Next, to bolster the security of the application, I added a login page, requiring the user to sign in with a username/password combination before being able to access the rest of the application. After that, I created text boxes that allowed the user to search for ranges of values in columns (rather than singular values), and then created an algorithm to combine the queries from the filters and the value ranges. Afterwards, I wanted to show off my ability to work with databases, so I converted the entire database to run off SQL instead of MongoDB. Finally, to bring the whole project together, I implemented the rest of the CRUD module (Create, Update, and Delete) in the application, creating separate pages that individually allow the user to create database entries, update values within existing database entries, and to delete existing database entries. In addition to all of that, I fixed the formatting issues and bugs contained in the original code.

The above changes were done in four installments: Enhancement One, Enhancement Two, Enhancement Three, and Final Project. The helper buttons and login page were implemented in Enhancement One. Enhancement Two consists of the changes made by Enhancement One in addition to the range search functionality. Enhancement Three is the first two enhancements, but it uses an SQL database instead of a MongoDB one. The Final Project is all three enhancements and the Create, Read, and Delete application capabilities. 

## Pre-Enhancement Code
Pre-enhancement code can be found [here](https://github.com/joshuarpickle/cs-499-code-milestones/tree/main/OriginalProject)

Application main function is located at ProjectTwoDashboard.ipynb

Application will not work as intended unless requirements detailed in **requirements.txt** and **additional-requirements.txt** are met

## Code Review
Below is the code review video for the pre-enhancement code:

[![Watch the video](https://img.youtube.com/vi/5mY87pMS58Q/0.jpg)]([https://www.youtube.com/watch?v=5mY87pMS58Q])

## A Quick Note
The following sections go over the versions the project went through during development along with my thoughts as the project progressed.

For those only interested in the project in its most recent, most complete state, go here

## Enhancement One Code
Enhancement One code can be found [here](https://github.com/joshuarpickle/cs-499-code-milestones/tree/main/EnhancementOneProject)

Application main function is located at ProjectTwoDashboard.ipynb

Application will not work as intended unless requirements detailed in **requirements.txt** and **additional-requirements.txt** are met

## Enhancement One Narrative
This project is a Jupyter Dash/MongoDB application that I worked with in CS 340: Client/Server Development in September through October of 2025. For this project, I was instructed to create a CRUD (Create, Read, Update, Delete) Python module for the database, as well as design very specific features for the page. 

I selected this application because I felt it would be a good starting point to work on in multiple different areas. As such, I intend for the enhancements to do most of the demonstrations of my skills and abilities in software development. In this milestone, I implemented a sign-in system for the application using the Flask-Login extension and designed a page for the user to input their credentials (username and password). I also created small “?” buttons next to potentially confusing items in the database page that, when hovered over, open pop-ups that appear to clarify what certain things are.

I believe I did meet the course outcomes I intended to meet with these enhancements. They were Course Outcomes #1 (Employ strategies for building collaborative environments that enable diverse audiences to support organizational decision-making in the field of computer science), #2 (Design, develop, and deliver professional-quality oral, written, and visual communications that are coherent, technically sound, and appropriately adapted to specific audiences and contexts), and #5 (Develop a security mindset that anticipates adversarial exploits in software architecture and designs to expose potential vulnerabilities, mitigate design flaws, and ensure privacy and enhanced security of data and resources). I do not currently have any changes to my outcome-coverage plans.

The main thing I learned from this set of enhancements was how to use documentation to my advantage. There were a lot of things I didn’t know how to do in JupyterDash before that I learned how to do looking through the documentation of various components in the Plotly Dash website. The challenges I faced were primarily due to my lack of experience in JupyterDash, but as previously mentioned, I got through primarily by checking documentation of various parts of the application.

## Enhancement Two Code
Enhancement Two code can be found [here](https://github.com/joshuarpickle/cs-499-code-milestones/tree/main/EnhancementTwoProject)

Application main function is located at ProjectTwoDashboard.ipynb

Application will not work as intended unless requirements detailed in **requirements.txt** and **additional-requirements.txt** are met

## Enhancement Two Narrative
This project is a Jupyter Dash/MongoDB application that I worked with in CS 340: Client/Server Development in September through October of 2025. For this project, I was instructed to create a CRUD (Create, Read, Update, Delete) Python module for the database, as well as design very specific features for the page.

I selected this application because I felt it would be a good starting point to work on in multiple different areas. As such, I intend for the enhancements to do most of the demonstrations of my skills and abilities in software development. In this milestone, I implemented a range-search capability to the application, allowing the user to search for ranges of values in select table columns, rather than the previous limitation the application had to only search for a specific query. 

I believe I did hit the course outcome I intended to hit with these enhancements. It was Course Outcome #3 (Design and evaluate computing solutions that solve a given problem using algorithmic principles and computer science practices and standards appropriate to its solution while managing the trade-offs involved in design choices). I do not currently have any changes to my outcome-coverage plans.

Luckily for me, this set of enhancements was rather smooth sailing for me, as I already happened to know a lot of the things that I needed to create them. I also had a very clear outline of what I wanted the program to do, and certain parts of the application that I had already created were a major help in simplifying any of the complexities that might’ve made the application more complicated and therefore harder to keep track of. Most of the challenge was just remembering slightly niche Python things, like how to check if a string can be turned into a float. I think the main thing I learned when creating these enhancements is how valuable looking at the current codebase for solutions - rather than just creating everything from scratch - can be. My initial intention was actually to create a whole new set of functions for the queries generated by the different text inputs, and then deal with deciding whether the queries from the pre-existing filter buttons should come before or after the queries from the text inputs, and then deal with any problems caused by potentially concurrent functions outputting to the same place… it was going to be a whole mess. Thankfully, I had the epiphany that I could just create one general query function starting with the existing query function from the filter buttons, and things became significantly simpler. 

## Enhancement Three Code
Enhancement Three code can be found [here](https://github.com/joshuarpickle/cs-499-code-milestones/tree/main/EnhancementThreeProject)

Application main function is located at ProjectTwoDashboard.ipynb

Application will not work as intended unless requirements detailed in **requirements.txt** and **additional-requirements.txt** are met

## Enhancement Three Narrative
This project is a Jupyter Dash/MongoDB application that I worked with in CS 340: Client/Server Development in September through October of 2025. For this project, I was instructed to create a CRUD (Create, Read, Update, Delete) Python module for the database, as well as design very specific features for the page.

I selected this application because I felt it would be a good starting point to work on in multiple different areas. As such, I intend for the enhancements to do most of the demonstrations of my skills and abilities in software development. In this enhancement, I changed the system to function off MySQL instead of MongoDB, completely changing the backend of the application to fit within the requirements of the database while adjusting to the new database system.

I believe I did meet the course outcome I intended to hit with these enhancements. It was Course Outcome #4: (Demonstrate an ability to use well-founded and innovative techniques, skills, and tools in computing practices for the purpose of implementing computer solutions that deliver value and accomplish industry-specific goals). Given that I believe I have covered all the course outcomes, I do not have any plans when it comes to covering outcomes. I did read the feedback for Milestone Two, so I’ll do some brainstorming with regards to furthering the software design aspects of the application. In addition, I intend to do some more polishing of the UI of the page.

The main challenge I faced when creating this milestone was the reduced amount of time I had to work on it due to life circumstances. For the most part, I only really had until Thursday night this week in terms of guaranteed time to work on the enhancements. As such, I had to learn how to deal with strict scheduling, which means figuring out ways to solve problems quickly without compromising code quality. In this scenario, that eventually meant dropping the “update()” method in the CRUD module, because it didn’t provide anything to the database (it’s a relic from the CS 340 class), and it was looking like it was going to take way too much time to migrate to something more SQL-friendly. However, I may bring it back when I have more time and might even implement it into the database.

## Final Project Code
The complete final project code can be found [here](https://github.com/joshuarpickle/cs-499-code-milestones/tree/main/FinalProject)

Application main function is located at GraziosoSalvareDashboard.ipynb

Application will not work as intended unless requirements detailed in **requirements.txt** and **additional-requirements.txt** are met
