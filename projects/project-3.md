---
layout: project
type: project
image: images/LogoC++.png
title: C++ Record Database
permalink: projects/DatabaseC++
# All dates must be YYYY-MM-DD format!
date: 2020-05-01
labels:
  - C++
  - VIM Editor
summary:  A robust record database that I coded in C++ for ICS 212.
---

<img class="ui image" src="{{ site.baseurl }}/images/Project2UI.png">

This project is a redesign of the C Record Database project, but written in C.  A thorough understanding of how C++ operates in terms of function calls, parameters, memory allocation, and scope is required to implement this.  Operator functions were defined for object handling, as well as a function that recursively prints the database and a function that reverses the order of the list.  Objects were now used in the linked lists to represent the records.  Although the functionality of this project mirrors the C Record Database, its implementation requires a much greater understanding of memory allocation, pointers, and how parameters work. Again, this was an individual assignment so a complete understanding of this content was required to implement the project.

This code sample is used to clean up object memory after the program finishes running:
```
 currentNode = this->start;

    while ( currentNode != NULL )
    {
        nextNode = (*currentNode).next;

        delete currentNode;

        currentNode = nextNode;
    }

    this->start = NULL;
```
