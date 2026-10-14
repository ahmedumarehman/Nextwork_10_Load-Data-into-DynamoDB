<img src="https://cdn.prod.website-files.com/677c400686e724409a5a7409/6790ad949cf622dc8dcd9fe4_nextwork-logo-leather.svg" alt="NextWork" width="300" />

# Load Data into DynamoDB

**Project Link:** [View Project](https://nextwork.ai/projects/8bd82466-f5ee-569e-9125-2c4c6ce7a07f)

**Author:** Ahmed Umar Rehman  
**Email:** ahmedumar475@gmail.com

---

![Image](https://nextwork.ai/calm_indigo_beautiful_lizard/uploads/8bd82466-f5ee-569e-9125-2c4c6ce7a07f_b481c730)

## Introducing Today's Project!

### What is Amazon DynamoDB?

Amazon DynamoDB is a non-relational (NoSQL) database service that organizes data using items and attributes. It is useful because it provides flexible data structures and fast access to items using partition keys.    Pasted text

### How I used Amazon DynamoDB in this project

In today's project, I used Amazon DynamoDB to create tables, load data into them using AWS CloudShell, and view and update the stored data.

### One thing I didn't expect in this project was...

One thing I didn't expect in this project is that i faced IAM Permission during creating tables or opening CLI 

### This project took me...

This project took me exactly 1 hour.

## Create a DynamoDB table

DynamoDB tables organise data using items and attributes. 

An attribute is a piece of data about an item in a DynamoDB table.

![Image](https://nextwork.ai/calm_indigo_beautiful_lizard/uploads/8bd82466-f5ee-569e-9125-2c4c6ce7a07f_a3cefee0)

## Read and Write Capacity

Read capacity units (RCUs) and write capacity units (WCUs) are units that measure how much read and write activity a DynamoDB table can handle per second.

Amazon DynamoDB's Free Tier covers 25 GB of data storage, plus 25 read capacity units (RCUs) and 25 write capacity units (WCUs). I turned off auto scaling because it could increase the table's processing capacity and potentially push usage beyond the Free Tier limits if not monitored.

![Image](https://nextwork.ai/calm_indigo_beautiful_lizard/uploads/8bd82466-f5ee-569e-9125-2c4c6ce7a07f_ef47dd8f)

## Using CLI and CloudShell

AWS CloudShell is a browser-based shell environment in the AWS Management Console that lets you run commands using the AWS CLI to manage AWS resources.

AWS CLI is a command-line tool that lets you create, manage, and interact with AWS resources using commands instead of the AWS Management Console.

I ran a CLI command in AWS CloudShell that created four DynamoDB tables: ContentCatalog, Forum, Post, and Comment.

![Image](https://nextwork.ai/calm_indigo_beautiful_lizard/uploads/8bd82466-f5ee-569e-9125-2c4c6ce7a07f_81e0258b)

## Loading Data with CLI

I ran CLI commands in AWS CloudShell that loaded data from all four JSON files into their matching DynamoDB tables.

![Image](https://nextwork.ai/calm_indigo_beautiful_lizard/uploads/8bd82466-f5ee-569e-9125-2c4c6ce7a07f_791c600b)

## Observing Item Attributes

![Image](https://nextwork.ai/calm_indigo_beautiful_lizard/uploads/8bd82466-f5ee-569e-9125-2c4c6ce7a07f_b481c731)

I checked a ContentCatalog item, which had the following attributes

Authors, ContentType, Difficulty, Price, ProjectCategory, Published, Title, URL

I checked another ContentCatalog item, which had a different set of attributes

ContentType, Price, Services, Title, URL, VideoType

## Benefits of DynamoDB

A benefit of DynamoDB over relational databases is flexibility, because each item can have its own unique set of attributes instead of every item needing the same columns.

Another benefit over relational databases is speed, because DynamoDB uses partition keys to quickly find the items it's looking for instead of scanning through the entire table.

![Image](https://nextwork.ai/calm_indigo_beautiful_lizard/uploads/8bd82466-f5ee-569e-9125-2c4c6ce7a07f_b481c730)

---

*Built with [NextWork](https://nextwork.ai) - [View this project](https://nextwork.ai/projects/8bd82466-f5ee-569e-9125-2c4c6ce7a07f)*
