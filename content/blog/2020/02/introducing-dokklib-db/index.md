---
title: "Introducing Dokklib-DB"
date: "2020-02-28"
---

I've released a new [Python library for the DynamoDB single table pattern](https://dokklib.com/libs/db/) called Dokklib-DB. It's built on top of Boto3 and should feel familiar if you've worked with Boto3 before.

Dokklib-DB addresses a few pain points I had while doing single table DynamoDB with Boto3:

1. I dislike constructing nested dicts for queries. These are error-prone and hard to test. With Dokklib-DB you pass Python objects as query arguments and get type/typo safety for primary keys and indices. ([Example of many-to-many queries](https://dokklib.com/libs/db/many-to-many/))
2. It's hard to keep track of the various entities and key patterns in the table. Dokklib-DB solves this by requiring key names to be special classes. This helps with documenting the entities and enforces a common prefix schema. ([Entity prefixes in the docs](https://dokklib.com/libs/db/table-setup/#entity-prefixes))
3. It's hard to handle errors with Boto3, especially with transactions, as it has dynamically generated exceptions which breaks static analysis for error handling, and raises all transaction errors as one generic error type. Dokklib-DB hard codes DynamoDB exceptions thus making static analysis possible and dispatches the specific transaction failure error exceptions.

You can find out more in the [Dokklib-DB docs.](https://dokklib.com/libs/db/)
