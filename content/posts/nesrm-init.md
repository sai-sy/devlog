+++
title = 'NESRM Init'
date = 2024-03-22T00:32:22-04:00
draft = false
tags = ["nesrm","nextjs","react","golang"]
categories = ["nesrm"]
projects = ["nesrm"]
+++
# NESRM | What and Why
The "Never Ever Stable" Relationship Manager is an idea that I've been mulling over for a while now. I have a very specific use case that most CRM's can't model for me, atleast cheaply. All the different ideas and tasks can get overwhelming, so I hope trying to write some of it down might help.

# The Challenges & Solutions
## 1. Database
A lot of this begins trivial. Personal data, family relatinships, it starts easy. Then you need to model that people will provide you different emails, and they are indeed the same person, or that people move houses, etc...  
The task gets large and unwieldy very fast so let's break down some tables
1. Person 
    - A basic table to model someones firstname, surname, deceased date, etc. This is the most basic non relational data someone might have... and the relational uuid for a mother and a father. All other genetic relationships can be modelled off of just a mother and father. 
2. Address
    - A list of every address in our database. Address formats are not consistent or pretty, so modelling this well but flexibly is important. 
3. Person-Address MtM relationship
    - A way to describe the relationship that exists, while also defining the last time this person has pinged that they live at that address. You could model deeper information like when someone bought and sold a property but that seems like more information that could ever be reasonably gathered, and would lead to useless columns


okay I realized writing this is blog is stressing me out more so screw the tables I will touch on that later

## 2. DB API
Don't do direct access. There is so much mess in these foreign keys it's not worth it. So many relationships to model. Let's have some fun and setup a GOLANG REST API to handle almost all the requests possible, and provide the data neccesary.

I'll define models and best practices in the readme for this

## 3. Auth
Figure out an auth system, each user for admin.nesrm.com needs to also be connected to a person row in the person table. forget aobut oAuth for now

## 4. Admin 
1. tables
2. auth permissions
3. managing tables 

## 5. admin/cutting lists
this god awful task

## 6. app.nesrm.com and the actual mobile canvas app

## 7. calling software? callhub listener? not sure

and I'm tired. but laying this out was nice
