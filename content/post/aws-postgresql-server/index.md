---
title: "Introduction to AWS PostgreSQL Server Documentation"
subtitle: "Introducing my documentation on creating a PostgreSQL server using an AWS EC2"
summary: "Introducing my documentation on creating a PostgreSQL server using an AWS EC2"
authors:
- admin
categories:
- Data-Science
date: "2021-02-06"
lastmod: "2021-02-06"
featured: false
draft: false

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Placement options: 1 = Full column width, 2 = Out-set, 3 = Screen-width
# Focal point options: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight
image:
  placement: 2
  caption: ''
  focal_point: ""
  preview_only: false

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects: []
---

Imagine the following scenario:

1. You have several files of data that are interconnected with each other

2. You want to create data tables combining information from separate data files

3. You want your project team to access the data and tables all from one location

A SQL server allows you to input your data into a database and create tables from different files using SQL commands, and you can also create users and allow them access to different databases in your server.

There's a big remaining question: how do you create a server for everyone in your project team to access? Several cloud vendors offer solutions, but most of the pre-configured SQL database cloud services can become expensive (if you'd like to investigate for yourself, Amazon Relational Database Services (RDS) lists their pricing for PostgreSQL here).

A cheaper solution is to install and create your own PostgreSQL server on an Amazon EC2 instance and having your teammates access the server through pgAdmin4, PostgreSQL's most popular GUI.

In this documentation,  we will

* Configure an AWS EC2 Ubuntu machine for PostgreSQL server
* Configure instance to scale up or down depending on CPU demand using EC2 auto-scale feature
* Set-up PostgreSQL server with users in our Ubuntu instance
* Access PostgreSQL server on our remote computers using pgAdmin4
* Backing up your PostgreSQL EC2 server in AWS

The goal is to review every step and give clear rationale so that you not only know what to do but also why you're doing it. Additionally, I list all of the website resources referenced in each section.

To access the rest of my documentation, visit the following site:

https://aws-postgresql-docs.beliciarodriguez.com/
