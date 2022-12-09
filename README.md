# C# .NET Live Project
## Introduction
As part of the curriculum at [The Tech Academy](https://learncodinganywhere.com), I worked as a full-stack developer for a two-week sprint - contributing to an MVC web application created with ASP .NET and Entity Framework. The work environment was based on an agile framework, complete with a sprint planning meeting, daily standups, and code retrospectives. The app serves as an interactive website for a local theatre in Seattle, designed as a Content Management System to allow users to manage their site to their liking, without technical knowledge.

The project allowed me to work in a legacy codebase, completing both front-end and back-end user stories, both contributing to a product that allows users to fill a database with Cast Members data, then read, or update/delete said data; implemeting full [CRUD functionality](#crud-functionality).

## CRUD Functionality
[CRUD](https://learn.microsoft.com/en-us/iis-administration/api/crud) refers to the four main functions inherent to relational databases. Implementing the four CRUD functions allows users of my Live Project to **c**reate, **r**ead, **u**pdate, and **d**elete data related to my cast members model.

## ***Below, I'll highlight some of the work I completed as part of the 10-day sprint.***

#### Story 1 
##### ***Back-end*** - Create an Entity Framework model that represents Cast Members and their associated data.
I was tasked with creating an entity model for my assigned class (Cast Members), an enum for their role in the theatre, and adding CRUD functionality. After the model was created and functional, I scaffolded the CRUD pages - creating  Index, Edit, Create, Details, and Delete pages. 

![A code snippet of the Cast Members model and its properties](https://github.com/jmternes/C-Sharp-Live-Project/blob/main/myModel.png?raw=true)

<hr/>

#### Story 2 
##### ***Front-end*** - Style the CRUD Pages.
After creating the CRUD pages, it was time to make some significant styling changes. These updates were based on requirements given to me by The Tech Academy, which included styling buttons, adding placeholders to the input fields, placing the form in a centered container, and adding borders to the input fields that matched the client's design desires. 

![A screenshot of the website's design](https://github.com/jmternes/C-Sharp-Live-Project/blob/main/CreatePage.png?raw=true)

<hr/>

#### Story 3
##### ***Back-end*** - Allow users to upload images from their own file systems for storage and retrieval.
This story provided many learning opportunities and new, useful knowledge moving forward. A user's image is uploaded from their system, then - in the controller - is converted into a byte[ ] and stored in the database. The image is then converted back into an image when retrieved for display in the views. 

###### ***This method converts the uploaded image into a byte[ ]:***

![A code snippet of the image to byte array method](https://github.com/jmternes/C-Sharp-Live-Project/blob/main/Image%20to%20Byte%5B%5D%20Method.png?raw=true)

###### ***Then, I called the above method within the Create and Edit views methods to convert the uploaded image to a byte[ ]:***

![A code snippet of the Create views method](https://github.com/jmternes/C-Sharp-Live-Project/blob/main/Image%202%20Byte%5B%5D%20Method%20Called.png?raw=true)

###### ***Lastly, I used [Razor syntax](https://learn.microsoft.com/en-us/aspnet/web-pages/overview/getting-started/introducing-razor-syntax-c) to get the byte[ ] from the Model, and convert it back to an image so the CSHTML img tag could render it:***

![A code snippet of the CSHTML file](https://github.com/jmternes/C-Sharp-Live-Project/blob/main/Display%20the%20Converted%20Image.png?raw=true)

<hr/>

#### Story 4 
##### ***Front and Back-end*** - Style the Index page with the Cast Members Model entries.
Since our Index page still had default styling, I was assigned to redesign the page to meet the requirements of the "design team". Using bootstrap cards and modals, I made a clickable image (that a user could [upload](#story-3)), labeled with the name property of the Cast Members model. I also added edit and delete options on the cards, improving the site's usability.

![](https://github.com/jmternes/C-Sharp-Live-Project/blob/main/IndexPage.png?raw=true)
*Note: the images are placeholders, but the user's uploaded image would display there.*

<hr/>

#### Summary
During this 10-day sprint with The Tech Academy, I got to work as a team member in a Scrum environment - completing front and back-end stories to contribute to a legacy codebase. I also got to practice version control, using Git within the Visual Studio IDE and Azure DevOps. I learned a lot of useful skills, both general and technical, and will take the skills and knowledge acquired with me moving forward.

<hr/>

###### ***Jump to: [Introduction](#introduction) | [Story 1](#story-1) | [Story 2](#story-2) | [Story 3](#story-3) | [Story 4](#story-4)***
