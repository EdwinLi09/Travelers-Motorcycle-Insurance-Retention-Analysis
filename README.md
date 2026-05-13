# Travelers Motorcycle Insurance Retention Analysis

## About This Project

This project was created as part of a team class assignment for Travelers Insurance, with the goal of helping the company keep more of its motorcycle insurance customers. Motorcycle insurance is different from regular car insurance because it tends to be seasonal, and many riders cancel during the off-season months when their bikes are stored away. On top of that, sudden price increases and bad claim experiences push riders to shop around with other insurance companies. Our team built a database and a set of SQL queries to help Travelers spot at-risk customers early and reach out to them before they decide to leave.

## The Problem We Were Trying to Solve

Travelers wanted a better way to understand why motorcycle riders were cancelling their policies and to figure out which customers were most likely to leave next. Without a clear picture of customer activity, rate changes, claims history, and outreach efforts in one place, it is hard to make smart retention decisions. Our project addressed this by pulling all of these pieces together into a single, organized database that the company could analyze and act on.

## Tools Used

The entire project was built using SQL and DBeaver. DBeaver is a database management tool that allowed our team to design the structure, add data, and run queries all in one workspace. We chose SQL because it is the standard language for working with relational databases, and it gave us a reliable way to ask questions of our data and pull out useful answers.

## How the Database Is Structured

The database is made up of nine tables, and each one focuses on a specific part of the motorcycle insurance business. The Customer table is the starting point and holds basic information about each rider. The Policy table connects each customer to the insurance products they own, and the Motorcycle table stores details about the bikes that are being insured. The PolicyTerm table tracks the lifecycle of each policy over time, including start and end dates along with the base premium charged.

To capture activity over the life of a policy, we built four supporting tables. The Claims table records the history of accidents or losses. The RateChangeEvent table keeps track of every time a premium goes up or down. The Payment table stores payment history, and the OutreachEvent table logs every time Travelers reaches out to a customer for retention purposes. Finally, the RiskAssessment table holds a calculated risk score for each policy, which is used to flag customers who may need extra attention.

All of these tables are connected through primary and foreign keys, which makes sure the data stays accurate and that each record can be traced back to the right customer and policy. Each table was filled with over 100 records so that the queries would produce meaningful results.

## What the Queries Do

The repository includes four SQL queries, and each one is designed to answer a different business question. The first query looks at high-risk policies that are coming up for renewal soon, so the retention team can step in before those customers cancel. The second query identifies policies that have had large rate increases combined with heavy claims activity, since those are the customers most likely to start shopping around. The third query analyzes which retention strategies and outreach methods have worked best in the past, giving the team a guide for what to do going forward. The fourth query groups customers by ZIP code and vehicle type to show where Travelers faces the highest risk and the most expensive coverage, which helps the company target pricing and outreach decisions by location and bike type.

## Why It Matters

The value of this project is that it gives Travelers a clear, reusable way to find at-risk customers before they cancel, send the right offers to the right riders at the right time, and focus retention efforts on the segments of the business that have the biggest impact. The database and queries were also designed to be flexible, so the same approach can be applied to other Travelers insurance products in the future.

## Team Members

This project was completed by a team of four students. Stewart Silva served as the Business Analyst, Javier Lares as the Data Architect, Kevin Arante as the Database Admin, and Edwin Li as the Data Analyst.
