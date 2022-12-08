# C# .NET Live Project
## Introduction
As part of the curriculum at [The Tech Academy](https://learncodinganywhere.com), I worked as a full-stack developer for a two-week sprint - contributing to an MVC web application created with ASP .NET and Entity Framework. The work environment was based on an agile framework, complete with a sprint planning meeting, daily standups, and code retrospectives. The app serves as an interactive website for a local theatre in Seattle, designed as a Content Management System to allow users to manage their site to their liking, without technical knowledge.

The project allowed me to work in a legacy codebase, completing both front-end and back-end user stories, both contributing to a product that allows users to [fill](#-create) a database with Cast Members data, then [read](#-read), or [update/delete](#-update-and-delete) said data; implemeting full [CRUD functionality](#crud-functionality).

## CRUD Functionality
CRUD (an acronym for Create, Read, Update, Delete) refers to the four main functions inherent to relational databases. Implementing the four CRUD functions allows users of my Live Project to create, read, update, and delete data related to my cast members model.



## ***Below, I'll highlight some of the work I completed as part of the 10-day sprint.***

#### Story 1 (back-end) - Create an Entity Framework model that represents Cast Members and their associated data.
I was tasked with creating an entity model for my assigned class (Cast Members), an enum for their role in the theatre, and adding CRUD functionality. After the model was created and functional, I scaffolded the CRUD pages - creating  Index, Edit, Create, Details, and Delete pages. 

![](https://github.com/jmternes/C-Sharp-Live-Project/blob/main/myModel.png?raw=true)

<hr/>

#### Story 2 (front-end) - Style the CRUD Pages.
After creating the CRUD pages, it was time to make some significant styling changes. These updates were based on requirements given to me by The Tech Academy, which included styling buttons, adding placeholders to the input fields, placing the form in a centered container, and adding borders to the input fields that matched the client's design desires. 

![](https://github.com/jmternes/C-Sharp-Live-Project/blob/main/CreatePage.png?raw=true)

<hr/>

#### Story 3 (back-end) - Allow users to upload images from their own file systems for storage and retrieval.
This story provided many learning opportunities and new, useful knowledge moving forward. A user's image is uploaded from their system, then - in the controller - is converted into a byte[ ] and stored in the database. The image is then converted back into an image when retrieved for display in the views. 

###### ***This method converts the uploaded image into a byte[ ]:***

![](https://github.com/jmternes/C-Sharp-Live-Project/blob/main/Image%20to%20Byte%5B%5D%20Method.png?raw=true)

###### ***Then, I called the above method within the Create and Edit views methods to convert the uploaded image to a byte[ ]:***

![](
