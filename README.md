# UiPath RPA Application 
**Overview**
This UiPath RPA (Robotic Process Automation) application is designed to automate the process of retrieving information about Udemy courses based on incoming emails. The application listens for emails with specific subjects and attachments, extracts data containing course names and prices, scrapes details from the Udemy website, performs currency conversion using an API, and organizes the data in an Excel sheet before sending it to the client. Additionally, the robot now includes a feature to check the account login status and log in with robot credentials if necessary.

**Features**
Email Listener:

Monitors incoming emails for a specific subject.
Processes emails with attachments containing course information.
Data Extraction:

Extracts course names and prices from email attachments.
Login Status Check:

Checks if the Udemy account is already logged in.
Logs out if the account is currently logged in.
Login with Robot Credentials:

Logs in using robot credentials if the account is not logged in.
Web Scraping (Udemy):

Navigates to Udemy website.
Scrapes course details, including name, description, price, instructors, rating, and status.
Currency Conversion:

Calls an API to convert course prices to Egyptian pounds.
Excel Sheet Management:

Writes the scraped data into an Excel sheet.
Splits data into two sheets based on the price - valid and invalid courses.
Email Notification:
Sends an email to the client with the Excel sheet attached.
Includes information about the courses in the client's currency.

This document provides a step-by-step guide to set up a Dispatcher and Performance on UiPath Orchestrator for the Udemy website. The process involves creating a folder named "Udemy" on Orchestrator and setting up a queue named "Courses" to efficiently manage and execute tasks
Assets: Udemy_URL	
and have the url of udemy (www.udemy.com)
