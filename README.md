# reference-cache

The reference codebase for the Federated ORC Exchange

## What is this about?

This project is a holds references platforms for accessing and incorporating the Federated ORC exchange database. Inside you will ( should ) find implementations in multiple languages and using multiple database platforms to import and manipulate the most recent version of the database.

## Okay - What is the Federated ORC exchange database then?

The Federated ORC Exchange database is a collection of ORC license based open content that has been prepared in a standard format for sharing across any number of backend services. The goal is to reduce duplication of activity and prevent a single source of failure causing a loss of the data. Submission systems should be robust enough to encouage creators and publishers to insert their own documentation. Lastly, we hope/expect that we'll see writer utilities make use of the dataset for lookup and attribution.

## How to help?

Submit a PR or an issue!

## Repository Contents

|Path|Contents|
|----|-----|
|structures|Detailed structural JSON documents for the exchange|
|src | Container for each of reference platforms|

## How to

### As a Programtic User

To begin using the database, select one of the federation endpoints from the [endpoints](endpoints.md) documentation and check out the github repository per the sites process. Each site should have a thorough how-to.

### As a Programatic Contributor

Reach out to the endpoint manager you collect from for a contribution ID.

To create an update contribution:

1. Ensure your database is up to date.
2. Create a new branch named in the format "YYYYMMDD_CONTRIBUTORID" 
3. Export/Update the branch with your changes.
4. Push your changes upstream.