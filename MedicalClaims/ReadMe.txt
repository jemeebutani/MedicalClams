# Medical Claim Reimbursement 

The purpose of a medical claim website is to provide a platform for Stakeholder to efficiently manage the process of submitting, reviewing, and processing medical claims. The website aims to streamline the claims process, reduce administrative burdens, and improve communication between all parties involved in medical billing and reimbursement. By providing a user-friendly and secure platform for submitting and managing medical claims, the website aims to improve the overall healthcare experience for patients and providers alike.

## Features and Functionalities

1. User Accounts: Stack Holder can create accounts to securely manage their medical claims and associated information.

2. Claim Submission: Patients can submit medical claims online, including information about the medical service provided, the healthcare provider.

3. Claim Tracking: Users can track the status of their claims, including any approvals or denials.

4. Auto Fill : Auto Fill is a feature that automatically populates form fields with pre-existing data or commonly used values.Auto Fill can save time and reduce errors by automatically filling in patient information.

## Technology Stack

The application is developed using React and the Flask programming language. The Firebase database is utilized for storing and retrieving the urls for bills uploaded and MySQL is used for storing the submitted form information and status of application from diffrent stakeholders, ensuring a robust and efficient system.

## Getting Started

To set up and run the application just follow this link: https://medical-claims-t17.netlify.app/

## To run the code files:

For frontend:
Open app directory in terminal and run ‘npm install’ to download all the dependencies.
Type ‘npm start’ to run the website.

To run the backend:
Run the following commands in order:
1. cd api
2. virtualenv venv
3. venv\Scripts\activate
4. pip install requirements.txt
6. python app.py
Server will run now.

To design database:
Open MySQL prompt and create a database named dep_2023_t17:
2. Then enter in that database.
3. Create the tables using the following commands:

a) CREATE TABLE application(application_id SERIAL PRIMARY KEY, user_id
VARCHAR(100) NOT NULL, page1 VARCHAR(1000), page2
VARCHAR(1000), page3 VARCHAR(1000), page4 VARCHAR(10000),
pharmacist VARCHAR(20),pharmacist_remarks VARCHAR(300), medical_officer
VARCHAR(20), medical_officer_remarks VARCHAR(300),DA_JAO
VARCHAR(20), DA_JAO_remarks VARCHAR(300),AO VARCHAR(20),
AO_remarks VARCHAR(300), Sr_AO VARCHAR(20), Sr_AO_remarks
VARCHAR(300), registrar VARCHAR(20), registrar_remarks VARCHAR(300),
director varchar(20), director_remarks varchar(300));

b) create table basicdetails(user_id varchar(100) primary key not null, data
varchar(1000));

c) create table data(application_id INTEGER NOT NULL, table_data
VARCHAR(1000) );

d) create table login(email varchar(30) NOT NULL);

## Conclusion

In conclusion, the development of a medical reimbursement website aims to streamline the claims process, reduce administrative burdens, and improve communication between patients and healthcare providers. With features such as claim submission and tracking,  the website will enhance the overall healthcare experience and improve the efficiency of medical claim management.

