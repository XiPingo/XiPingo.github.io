---
layout: post
title: Introduction to Databases
date: 2025-08-27 14:00 +0800
last_modified_at: 2025-12-26 12:00 +0800
tags: computer
toc:  true
math: true
---
Welcome to the homepage of **Introduction to Databases** !   
Tips: As a cultural form, database represents the world as a list of items and it refuses to order this list. In contrast, a narrative creates a cause-and-effect trajectory of seemingly unordered items (events). Therefore, database and narrative are natural enemies.   
——Lev Manovich
{: .message }

# Course Introduction

<mark>Course number: 22020250 Credit: 3</mark>   

The teaching content of this course is as follows:   

<table border="1" width="100%">
  <tr>
    <th>Week</th>
    <th>Content</th>
  </tr>
  <tr>
    <td>1</td>
    <td>
      <ul>
        <li>Course Introduction: Overview, Requirements, and Assessment</li>
        <li>Chapter 1: Database System Overview
          <ul>
            <li>1.1 Basic Concepts: Data, Database, DBMS, Database System, DBA</li>
            <li>1.2 History and Current Status of Database Systems</li>
            <li>1.3 Core Features: Data Integration, Independence, Sharing, Redundancy, Security, Integrity, Consistency, Concurrency Control, and Recovery</li>
            <li>1.4 Relational Database Architecture: Three-Schema Architecture and Two-Level Mappings</li>
          </ul>
        </li>
        <li>Chapter 2: Data Models
          <ul>
            <li>2.1 Basic Concepts: Data Model Definition, Components, and Classification</li>
            <li>2.2 Three Categories of Data Models and Their Relationships</li>
            <li>2.3 Conceptual World and Conceptual Data Models (Part 1)
              <ul>
                <li>Conceptual Data Models and Classification</li>
                <li>Entity-Relationship (ER) Model Overview</li>
                <li>Entities, Entity Sets, Attributes, and Keys</li>
                <li>Relationships: Definition, Classification, and Cardinality</li>
              </ul>
            </li>
          </ul>
        </li>
      </ul>
    </td>
  </tr>
  <tr>
    <td>2</td>
    <td>
      <ul>
        <li>2.3 Conceptual World and Conceptual Data Models (Part 2)
          <ul>
            <li>ER Model Design Methodology and ER Diagrams</li>
            <li>ER Model Design Cases and Graphical Representation</li>
            <li>Extended ER Model and Its Visualization</li>
            <li>Object-Oriented and Predicate Data Models</li>
          </ul>
        </li>
        <li>2.4 Logical Model: Basic Concepts of Relational Data Model</li>
        <li>2.5 Physical Model: File Organization and Indexing Basics</li>
      </ul>
    </td>
  </tr>
  <tr>
    <td>3</td>
    <td>
      <ul>
        <li>Chapter 3: Relational Database Systems
          <ul>
            <li>3.1 & 3.2 Advantages and Criteria of Relational Databases</li>
            <li>3.3 Relational Model Theory
              <ul>
                <li>Basic Concepts: Terminology, Relations, Constraints, and Data Manipulation</li>
                <li>Relational Algebra (Part 1): Five Basic Operations, Extended Operators (Intersection, Join, Division), and Applications</li>
              </ul>
            </li>
          </ul>
        </li>
      </ul>
    </td>
  </tr>
  <tr>
    <td>4</td>
    <td>
      <ul>
        <li>Relational Algebra (Part 2): Comprehensive Applications and Summary</li>
        <li>Relational Calculus (Part 1): First-Order Predicate Calculus Basics, Atomic Formulas, and Closed-World Assumption</li>
      </ul>
    </td>
  </tr>
  <tr>
    <td>5</td>
    <td>
      <ul>
        <li>Relational Calculus (Part 2): Queries (Single-Table, Multi-Table Joins), Complex Queries (Negation, Implication), and Equivalence with Relational Algebra</li>
        <li>3.4 Relational Database Language SQL (Part 1): Introduction, Data Types, Table Creation, Basic Queries, Joins, and Self-Joins</li>
      </ul>
    </td>
  </tr>
  <tr>
    <td>6</td>
    <td>
      <ul>
        <li>National Day Holiday (No Class)</li>
      </ul>
    </td>
  </tr>
  <tr>
    <td>7</td>
    <td>
      <ul>
        <li>3.4 Relational Database Language SQL (Part 2): Subqueries, Correlated Queries, Division in SQL (NOT EXISTS), Aggregate Queries (GROUP BY, HAVING), and Comprehensive Applications</li>
        <li>3.4 Relational Database Language SQL (Part 3): Data Modification (INSERT, DELETE, UPDATE), Transactions, Views (Creation, Deletion, Updatability), and Query Rewriting</li>
      </ul>
    </td>
  </tr>
  <tr>
    <td>8</td>
    <td>
      <ul>
        <li>Chapter 4: Database Security and Integrity
          <ul>
            <li>4.1 Database Security: Concepts, Authentication, Access Control, and SQL GRANT/REVOKE</li>
            <li>4.2 Database Integrity: Entity, Referential, and User-Defined Constraints; SQL Constraints (PRIMARY KEY, FOREIGN KEY, CHECK, UNIQUE, NOT NULL, DEFAULT); Assertions and Triggers</li>
          </ul>
        </li>
      </ul>
    </td>
  </tr>
  <tr>
    <td>9</td>
    <td>
      <ul>
        <li>Chapter 6: Data Exchange in Databases
          <ul>
            <li>Embedded SQL: Programming, Cursors (Definition, Opening, Fetching, Closing), Updatable Cursors, and Exception Handling</li>
            <li>Programmable SQL (PL/SQL, T-SQL), Stored Procedures, and Functions</li>
            <li>Driver-Based Database Access Interfaces</li>
          </ul>
        </li>
      </ul>
    </td>
  </tr>
  <tr>
    <td>10</td>
    <td>
      <ul>
        <li>Chapter 8: Relational Normalization Design
          <ul>
            <li>Introduction: Data Redundancy, Anomalies, and Functional Dependencies</li>
            <li>Armstrong's Axioms (Part 1): Functional Dependency Classification, Axiom Rules, and Applications</li>
          </ul>
        </li>
      </ul>
    </td>
  </tr>
  <tr>
    <td>11</td>
    <td>
      <ul>
        <li>Armstrong's Axioms (Part 2): Logical Implication, Attribute Closure, and Key Calculation</li>
        <li>Normal Forms: 1NF, 2NF, 3NF, BCNF – Definitions, Relationships, and Decomposition Methods</li>
      </ul>
    </td>
  </tr>
  <tr>
    <td>12</td>
    <td>
      <ul>
        <li>Multivalued Dependencies and 4NF: Definitions, Rules, and Decomposition</li>
        <li>Armstrong's Axioms Supplement: Minimal Cover, Schema Decomposition (Lossless Join, Dependency Preservation), and Normalization Case Studies</li>
      </ul>
    </td>
  </tr>
  <tr>
    <td>13</td>
    <td>
      <ul>
        <li>Chapter 9: Database Design (Part 1)
          <ul>
            <li>9.1 Database Design Overview: Tasks and Lifecycle</li>
            <li>9.2 Requirements Analysis: Methods and Documentation</li>
            <li>9.3 Conceptual Design: ER Model, View Integration, and Case Studies</li>
          </ul>
        </li>
      </ul>
    </td>
  </tr>
  <tr>
    <td>14</td>
    <td>
      <ul>
        <li>Chapter 9: Database Design (Part 2)
          <ul>
            <li>9.4 Logical Design: ER-to-Relational Model Mapping</li>
            <li>9.5 Physical Design: Storage Structures, Indexing, and Access Paths</li>
            <li>9.6 Comprehensive Database Design Case Study</li>
          </ul>
        </li>
      </ul>
    </td>
  </tr>
  <tr>
    <td>15</td>
    <td>
      <ul>
        <li>Chapter 7: Database Physical Organization
          <ul>
            <li>Storage Media and File Organization</li>
            <li>Indexing Techniques: Dense/Sparse Indexes, Multilevel Indexes</li>
            <li>B+ Tree Indexes: Structure, Operations, and Comparison with B-Trees</li>
          </ul>
        </li>
      </ul>
    </td>
  </tr>
  <tr>
    <td>16</td>
    <td>
      <ul>
        <li>Chapter 5: Transaction Processing (Part 1)
          <ul>
            <li>Transactions: ACID Properties, States, and Isolation Levels</li>
            <li>Concurrency Control: Schedules, Data Inconsistencies, Locking (X-Locks, S-Locks), Two-Phase Locking, and Multigranularity Locking</li>
            <li>Deadlock Detection and Resolution</li>
          </ul>
        </li>
      </ul>
    </td>
  </tr>
  <tr>
    <td>17</td>
    <td>
      <ul>
        <li>Chapter 5: Transaction Processing (Part 2)
          <ul>
            <li>Database Recovery: Failure Types, Recovery Techniques (Backup, Logging, Mirroring)</li>
            <li>Transaction Logs: UNDO, REDO, and UNDO/REDO Logs – Recovery Workflows and Tradeoffs</li>
            <li>Recovery Strategies for Different Failure Scales</li>
          </ul>
        </li>
      </ul>
    </td>
  </tr>
  <tr>
    <td>18</td>
    <td>
      <ul>
        <li>Course Summary and Review</li>
      </ul>
    </td>
  </tr>
</table>

-----

# Course Resourse

## Textbook of Introduction to Databases

 [Textbook](https://xuanshu.hep.com.cn/front/book/findBookDetails?bookId=59cc8b39ba9eb884cf817620).
 

All rights reserved by 高等教育出版社.

-----

## Courseware of Introduction to Databases

 Email me if you need.   

 All rights reserved by Professer [Bai Wenyang](https://cs.nju.edu.cn/c9/4d/c2640a51533/page.htm).


-----

## Tips of Management

The course content is extensive, and the final exam preparation is highly stressful, but the teachers are very friendly.

-----