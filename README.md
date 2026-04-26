This is a HRMS Backend application that combines many human resources functions.It provides opportunities for the HR agents of a company to manage employees, departments, jobs and job seekers. The HR agent can view the list of all employees using filters, for example viewing a list of employees of a particular department. Create, delete or edit employee records in the system. Manage the company position, such as creating, updating, or deleting job offers. Manage payrolls of the employee.
📜 Project Main features

Our backend is powered by 5 microservices, all of which happen to be written in java using Spring Boot and JavaScript using NodeJS.
Employees Service: Provides PIM (Personal information management for employees and candidates). Provides employees information like hiring date, email, role, date of birth etc.
Recruitment Service: Provides recruitment information like Job Postings, Job Applicants etc.
Position Service: Provides postion information like designation, department name, employees etc.
Payroll Service: Provides payroll information like salaries etc.
Holiday/Leave Service: Provides holiday or leave information. Managing leave and defining holidays.
📐 Project Technical Architecture

Our sample microservices-based system consists of the following modules:
gateway-service : a module for running Spring Boot application that acts as a proxy/gateway in our architecture.
config-service : a module that uses Spring Cloud Config Server for running configuration server in the native mode. The configuration files are placed on the classpath.
discovery-service : a module thats Spring Cloud Eureka as an embedded discovery server.
employee-service : a module containing the 1st microservice that allows to perform CRUD operation on in-memory repository of employee.
payroll-service : a module containing the 2nd microservice that allows to perform CRUD operation on in-memory repository of payrolls. It communicates with account-service.
recruitement-service : a module containing the 3rd microservices that allows to perform CRUD operation on in-memory repository of recruitements.
position-service : a module containing the 4th microservices that allows to perform CRUD operation on in-memory repository of positions.
leave/holiday-service : a module containing the 5th microservices that allows to perform CRUD operation on in-memory repository of leave and holidays.

⚡ Usage

Use this space to show useful examples of how a project can be used. Additional screenshots, code examples and demos work well in this space. You may also link to more resources.
🚩 Roadmap


 Phase 1 : Implementation of Discovery and Gateway services

Implementation of Eureka as a discovery server
Implementation of Zull as a gateway or proxy server
Implementation of config server

 Phase 2 : Implementation of the main application microservices

Employees Service
Recruitment Service
Position Service
Payroll Service
Leave/Holiday Service

 Phase 3 : Deployement of microservices using Docker

