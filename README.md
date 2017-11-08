# SurveyWeb
This project is created in hope of creating a tool that can collect stats for any given object in the most effective way through different methods for various nodes in a given area and at different levels (Each node can be an a village or a town or an area in a town or a district etc). 

In the end, I want to make such tool available for NGOs or the government to take required initiatives to solve the issues. 

The approach I thought is :
 - To create domain type objects
 - Three such main objects: Problem Domain, Country Domain and Source Domain
 - Country Domain is a nested domain and consists of domain objects like Village, Town, District, Area etc. We can also call any of this domain object as 'Node'. 
 - Problem Domain can be a nested domain, but not necessarily. To simplify things, it is not nested and it's entries are not treated as domain. Each entry is a simple object that represents an 'Issue/Problem' like Malnutrition, Illetaracy, Poverty, Pollution etc.
 - We create mappings from Problem Domain to Country Domain.
 - Thus each mapping represents that a node (i.e., village or town or district) has a Issue. 
 - The mappings can have serveral properties: "Severity", "Authenticity", "Last Refresh" etc.
 - Severity is an integer with predefined values. Authenticity is integer that acts like a counter. 'Last Refresh' is DateTime representing Last Time when a Severity or Authenticity property is changed.
 - Source Domain consists of different source objects which creates the mappings or changes it's values. 
 - These source objects can be Field Survey (which has more added Authenticity for a mapping), Social Network Survey, Web Survey etc.
 - Some source objects like Social Network Suryey also has a key property called 'Location' i.e., the living-place/home-town of the person.
 - The idea is to create an an application for each social network site in which the person, while can create a mapping, can also send request for all his friends to create mappings.
 
 I am not from developing background. Also, I do not have an idea on project management. However, I have experience with Python, Unix Scripting and a bit C.
 
 The above is just my idea. Any other approach is also appreciable. 
 I am looking for people who can be part of this project, create the methods and frameworks, manage the projec and make it real. 
 

