

3] storage and databases
---

data storage intro
---
- unstructured data
    -> Google Cloud Storage
    - examples:
        - videos, blobs, ...

- structured data
    - analytics (for analysis)
        - low latency -> Cloud BigTable
        - high latency -> Cloud BigQuery
    - not analytics
        - relational
            - scalability important -> Cloud Spanner
            - not scalable -> Cloud SQL (Postgre/MySQL)
            - scalability = 
                - horizontal scaling, 
                - available over the world
                - consistency
        - not relational
            - Mobile SDK -> Cloud Firestore
            - NoSQL      -> Cloud Firestore
            - Cloud Firestore is a new ver of Coud Datastore
    - Cloud Memorystore
        -> Cloud Redis serv
            - key-value


working with data
---
- three basic stages for data modelling (~1.45)
    - conceptual stage
        - entities
        - attributes
        - relationships
    - logical
        - entity structures
        - can be normalized?
    - physical
        - implementation level
        - what database
        - which keys and indexes


data pipelines
---
- source
    - application
    - storage event
- ingest
    - pub/sub topic
- pipeline
    - dataflow (does some data transform)
    - bigquery (data accumulation)
- analytics
    - data studio (visualisation)


cloud storage transfer service
---
- automates the data transefer source->sink

- sink
    - Cloud Storage bucket (always)
- sources
    - AWS S3
    - http://
    - oteher google cloud storage buckets

- BigQuery data transfer service
    - sink
        - BigQuery
    - sources
        - google marketing platform
            - ads,youtube,..


cloud firestore
---
- replaced the older Coud Datastore
- pandan to aws dynamo db
- working with data (python) explained @ ~5:00




6] pipelines with cloud dataflow
---

cloud data flow
---
- uses apache beam sdk


- tips
---
- preferred solutions for:
    - batch workloads
        - dataproc
        - sparc
    - streaming data
        - beam
        - dataflow


- chapter 19
- Dataprep
