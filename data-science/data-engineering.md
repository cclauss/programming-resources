[CS329 - Lecture 3 - Data Engineering](https://docs.google.com/document/u/1/d/1b9iuZiDEGVLHyMmnf6w2y1aN6yWQhAyqk3GHlpI9q6M/mobilebasic)


[andkret/Cookbook](https://github.com/andkret/Cookbook) - The Data Engineering Cookbook
- hit and miss, early chapters are better

[Top 10 blog posts to help you transition to data engineering](https://blog.insightdatascience.com/top-10-blog-posts-to-help-you-transition-to-data-engineering-1db2312ecdaf)

`mara/mara-pipelines` - a lightweight data transformation framework with a focus on transparency and complexity reduction [github](https://github.com/mara/mara-pipelines)


## [Stanford Seminar - Big Data is (at least) Four Different Problems](https://youtu.be/S79-buNhdhI)

Michael Stonebreaker - created first RMDBS INGRES

Big data
- volume
- velocity
- + one other?

Where will there be disruption in the big data market

Data science versus BI analytics
- BI analytics = SQL
- petascale SQL is a solved problem
- 500+ nodes, databases work well

Column stores are faster (compression on the columns)
- all databases offer this
- performance + maturity + reliability differs a lot between offerings

Warehouses are getting faster than resources are getting cheaper

Data scientists will replace BI
- predictive model or big table of numbers
- BI = big table of number

Take a decade to train enough data scientists

Data science
- data management - SQL (table) based calcs
- complex analytics - array based calcs

Example of calculating covariance between many stocks
- equivalent to `stock * stock.T`
- not a table calculation

### How to support data science

Option 1
- Map Reduce + HDFS (2008)
- dropped by Google in 2011 -> BigTable
- 2015 officially abandoned

2013
- MapReduce is mostly SQL market (Hive)

Option 2
- spark

Spark
- no persistence
- no sharing (data is copied)
- no indexes
- 70% is SQL
- moves the data to the query (problem)

Option 3
- move query to data
- use relational database for SQL
- user defined functions for analytics
- table to arry is expensive

Option 4
- use array based DMBS
- most efficient long term solution

https://youtu.be/S79-buNhdhI?t=1849

Big velocity
- complex event processing





## Daniel Molnar talks

Berlin Buzzwords 2016
- [slides](https://www.slideshare.net/soobrosa/migrating-a-data-stack-from-aws-to-azure-via-raspberry-pi)
- [talk](https://www.youtube.com/watch?time_continue=378&v=QhXPANTd9nE&feature=emb_logo)

Data Janitor 101 - [slides](https://www.slideshare.net/soobrosa/data-janitor-101)

emphasis on data quality

KPIs that matter
- DAU, WAU, MAU, LTV, churn
- cohorts, segments, funnels
- first hour, first day

KPI should show you where the problems are

Actionable

Excel = most used programming environment
- no version control, ugly

business analyst ->  data engineer
- not real time / stream at the start

data engineer = entinty recognition
- ETL, events, data warehouse
- know where your data is leaking
- testing - unit test data

- you will see noise

a/b
- don't a/b test (unless it really makes sense)
- costs too much
- world isnt IID
- random variation in small samples
- most results are illusory
- small data -> bayesian


lots of data science is about proving something isn't working
- importance of curiosity, talking to users
- causation versus corrulation







- computers are a sadness, I am the cure
- chose boring technology
- discovering python
- you suck at excel, data driven products now!
- chris stucchio on testing
