# hands-on-lab-neo4j-and-sagemaker
Neo4j is the [leading graph database](https://db-engines.com/en/ranking/graph+dbms) vendor.  We’ve worked closely with AWS Engineering for years.  Our products, Neo4j Graph Database, Graph Data Science and Bloom are offered in the [AWS Marketplace](https://aws.amazon.com/marketplace/seller-profile?id=23ec694a-d2af-4641-b4d3-b7201ab2f5f9).

In this hands on lab, you’ll get to learn about Neo4j and Amazon SageMaker.  The lab is intended for data scientists and data engineers.  We’ll walk through deploying Neo4j and SageMaker on AWS in your own AWS account.  Then we’ll get hands on with a real world dataset, building a machine learning pipeline that takes advantage of features generated using Neo4j Graph Data Science to improve prediction in Amazon SageMaker.  You’ll come out of this lab with enough knowledge to apply graph feature engineering to your own datasets.

We’re going to analyze the quarterly filings of asset managers with $100m+ assets under management (AUM).  These are regulatory filings made to the Securities and Exchange Commission’s (SEC) EDGAR system.  We’re going to show how to load that data from an AWS S3 bucket into Neo4j.  We’ll then explore the relationships of different asset managers and their holdings using the Neo4j Browser and Neo4j’s Cypher query language.

Finally, we’ll use Neo4j Graph Data Science to create a graph embedding from our data, export that out, and run supervised learning algorithms in Amazon SageMaker.  We’ll try to predict what holdings asset managers will maintain or enlarge in the next quarter.  

If you’re in the capital markets space, we think you’ll be interested in potential applications of this approach to creating new features for algorithmic trading, understanding tail risk, securities master data management and so on.  If you’re not in the capital markets space, this session will still be useful to learn about building machine learning pipelines with Neo4j and Amazon SageMaker.

## Venue
These workshops are organized onsite in an AWS office.

## Duration
3 hours.

## Prerequisites
You'll need a laptop with a web browser. Your browser will need to be able to access the AWS Console and port 7474 on a Neo4j deployment running in AWS.  If your laptop has a firewall you can't control on it, you may want to bring your personal laptop.

If you have an AWS account already, you may be able to use that.  You would need permissions that allow you to deploy a SageMaker domain and deploy a CloudFormation template from Marketplace.  It would also need permission to deploy various AWS resources including a VPC and a Load Balancer.  If your access doesn't meet those requirements, we'll walk you through creating a new account with full access.

## Agenda

### Part 1
* Introductions
* Lecture - [Introduction to Neo4j](https://docs.google.com/presentation/d/1-wrPfSdyx-5qvFKX29BvpN-K-uWAOYEqYzz6J4LA30U/edit?usp=sharing) (15 min)
    * What is Neo4j?
    * Customer use cases
    * How is it deployed and managed on AWS?
* [Lab 0 - Signup for AWS](Lab%200%20-%20Signup%20for%20AWS) (15 min)
    * Improving the Labs
    * Signup for AWS
    * Apply AWS Credits
* [Lab 1 - Deploy Neo4j](Lab%201%20-%20Deploy%20Neo4j) (15 min)
    * Deploy Neo4j Enterprise Edition through the Marketplace
    * CloudFormation Template
* [Lab 2 - Connect to Neo4j](Lab%202%20-%20Connect%20to%20Neo4j/README.md) (15 min)
    * Neo4j Browser
    * Neo4j Bloom
    * Interacting via Shell
* Break (5 min)

### Part 2
* [Lecture - Moving Data](https://docs.google.com/presentation/d/1iAMN6o-aMNtg2WAZzHORbckV--JXa2wiY5YLBNDRN3w/edit?usp=sharing) (10 min)
    * LOAD CSV
    * Amazon Elastic Map Reduce (EMR)
    * Amazon Managed Streaming for Kafka
* [Lab 3 - Moving Data](Lab%203%20-%20Moving%20Data/README.md) (15 min)
    * A Day of Data
    * A Year of Data
* [Lab 4 - Exploring Data](Lab%204%20-%20Exploring%20Data/README.md) 10 min)
    * Vizualization with Neo4j Bloom
* Break (5 min)

### Part 3
* [Lecture - SageMaker](https://docs.google.com/presentation/d/1pbbYsA6U1RlTt5CJV6zjpDLya9xVThRODAO3-CyKIBc/edit?usp=sharing) (10 min)
    * What is SageMaker?
    * Using SageMaker with Neo4j
* [Lab 5 - SageMaker](Lab%205%20-%20SageMaker) (15 min)
    * Create a SageMaker Domain
    * Import from GitHub to SageMaker Studio
    * Pandas
    * Cypher
* Break (5 min)

### Part 4
* [Lecture - Graph Data Science](https://docs.google.com/presentation/d/1dx5ve401iHlUseznhdbHE-h-Uk97ENheS_d6tEVIcOc/edit?usp=sharing) (10 min)
    * Why Graph Data Science
    * Similarity
    * Centrality
    * Community Detection
    * Graph Machine Learning
    * Using SageMaker with Neo4j
* [Lab 6 - Graph Data Science](Lab%206%20-%20Graph%20Data%20Science/README.md) (15 min)
    * Create a Graph Embedding
    * Autopilot on Embeddings
    * Autopilot on Raw Data
* [Lab 7 - Cleanup](Lab%207%20-%20Cleanup) (15 min)
* [Discussion - Questions and Next Steps](Discussion%20-%20Questions%20and%20Next%20Steps.md) (5 min)
