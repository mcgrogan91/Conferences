# Grubhub Data Platform

## Grubhub data and use cases
Ecommerce application: 19 million diners, 520k a day. Ratings, reviews.
Drivers and Delivery: Logistics, Time sensitive, ETA prediction
	-	As more information comes into the order, the ETA can get better and better
Promotions: New customer, restauraunts, etc
CRM campaigns ():
Restauraunts:
	- Business to Business
	- 115k restauraunts
	- Rankings
Catalog/Content: 
	- Restauraunt classification
	- Menu and updates
	- Classifying menus


Microservices based. Large cassandra, milti-datacenter


## Challenges
![Picture](/PTW Dev Conference/images/Challenges.jpg)

## Overview of current architecture

![Picture](/PTW Dev Conference/images/Architecture.jpg)

Grubhub Data Platform Philosophy - SIMs
	- Scalability
	- Isolation of jobs
	- Managed self-service
	- Serverless*

(Took a picture of architecture)
Red: Self service capability
Inspiration came from Netflix
Why is this dude asking questions in the middle of the presentation?
Why is this other dude asking questions in the middle of the presentation?


## Self Service capabilities

100% cloud data platform

Why spark?
	- scalability
	- flexibility
	- performance
	- ecosystem support

Why presto?
 - Fast interactive query capability
 - Ability to connect to multiple platforms
 - Enterprise Presto with Apache Ranger

Why S3?
 - Seperating storage and compute layers
 	- Dynamic transient clusters
 - Scalability
 - Encryption
 - Access controls
 - Data redundancy
 - Retention policies
 - Data formats
 	- Parquet/ORC/Avro data formats

Managed self-service system
Automated job deployment
Cluster resources optimization/re-routing
Job dependency tracking (!!!!)
Data lineage tracking (!!!!!)

## Lessions Learned

- Good Data Modeling matters
	- Use Dimensional modeling where it makes sense
	- It helps users formulate their analytics queries
	- Better performance
	- Consistent source of truth
	- Hides underlying data complexity
- Complex Data Type in Analytics environment
	- Unstructured data
	- Complex Data Type getting better support
- Spark is great, but not for everyone and not for all use cases
	- end users are used to SQL, which is why they use Presto too
- Enterprise Presto for fine frained user access controls and security
SQL, Presto SQL, Spark SQL have differences



