+++
title = 'Database Front End Init'
date = 2024-03-21T14:15:03-04:00
draft = true
tags = ["nesrm","python","flask","database","postgresql"]
categories = ["nesrm","nesrmfe"]
+++
# First Step for the "Never Ever Stable" Relatinship Manager
NESRM will hopefully be a tool for me to manage the thousands of contacts I've built over the course of my campaigning work. Managing voter history, residence change, deceased parties, etc... has become a hassle. So I plan to do something about it. This is the front end preview for the database

## A Non-Final Solution
NESRM has many parts, and I need a way to see how those parts affect my data. Supabase is great, but looking at foreign keys is annoying. I want a proper CRUD interface to see my tables and how the rows relate to another another. To do so, I'll build a simple flask application to interface with the database, and present all the tables to me. That way I can show my progress and manage the program actions.

## Auth?
Now what to do about auth? I want to leave the supabase auth alone for now, so maybe I'll just spin up a linode isntance for a couple users. That adds another damn server to keep track of but I'd rather leave production tools like suapbase auth for production products. 

## ORM
Forget an ORM. But also I can't be asked to manange SQL queieres. I can't even spell query. So I'll define my own models with queries to use. This will be an ongoing pattern. Building classes as a baby internal ORM.

## Next Steps
Start building. Start a flask project. Build the interface away. And lets find out what we can do with this data.
