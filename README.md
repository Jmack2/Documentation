## Documentation
As a part of my Tutorial with the Computer Science Department at the College of Charleston for the fall semester 2016, I have created documentation for the ET_Redux, CHRONI, and Topsoil projects under Cyber Infrastructure Research & Development Lab for the Earth Sciences and published the documentation to the [CIRDLES](http://cirdles.org) website. Now, I periodically update the documentation along with the corresponding software. The template for the documentation was built based on information from Ian Sommerville's book **Software Documentation**. Ian Sommerville stated how important it is to consider the universal nature of the documentation:

>1. They should act as a communication medium between members of the development team.
>2. They should be a system information repository to be used by maintenance engineers.
>3. They should provide information for management to help them plan, budget and schedule the software development process.
>4. Some of the documents should tell users how to use and administer the system.

In addition to these broader requirements, the documentatin is specifically designed for users:

>Users of a system are not all the same. The producer of documentation must structure it to cater for different user tasks and different levels of expertise and experience. It is particularly important to distinguish between end-users and system administrators

However, this documentation needed to be accomodating for all skill levels, as well as end-users and system administrators. The end-user will need the documentation in order to specifically use the software and system administrators must use the documentation to manage the software. Since CIRDLES software is open source, this is a unique situation that allows users to directly interact with system administrators or make their modifications to the software almost like informal system administrators.

##Using the Template
The documentation template structure was built by using certain components listed in Sommerville's book, which are the Introduction, Information for use of Documentation, Concept of Operations, Procedures, and Glossary sections as seen below.

```markdown
###Template for User Documentation (Functional Description)
-Introductory Manual: informal introduction to system, describing normal usage

###Introduction to Software
-Purpose of Software -When and who created software -Brief summary of the contents

###Information for use of Documentation
-suggestions for different readers on how to use the documentation effectively\s\s
(e.g. there are videos for auditory and visual learners, step by step instructions on the website, etc.)

###Concept of operations
-An explanation of the conceptual background to the use of the software.

###Procedures
-Basic written instructions -Youtube videos -Directions on how to use the software<br> to complete the tasks that it is designed to support.

###Glossary
-Definitions of specialized terms used.
```
Users can customize this template by adding their own content to the given sections, remove certain sections, or add new sections to the template when they fork this repository.

##Publishing your Content
After original content has been added to the template, the user can try different methods to publish their documentation. The CIRDLES website requires different parts of the menu hierarchy to function as different pages, which explains why each section needs its own file. Therefore, you must copy and paste each section of the documentation into seperate files if this is how the hierarchy of your website functions. For example, the Introduction to Software section should have its own file, Concept of Operations should have its own file, etc.

Additionally, users can use GitHub Pages to create a branch called gh-pages in your repository. Github will build the site automatically and your site will be published at http://yourusername.github.io/repositoryname/. If you would like to have your website hosted elsewhere, than you can look at [Jekyll](http://import.jekyllrb.com/docs/home/) documentation for more information.
