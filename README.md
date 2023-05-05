<a name="readme-top"></a>

<!-- PROJECT TITLE AND LOGO -->
<br />
<div align="center">
  
   <h3 align="center">Replicating PostgreSQL Database to Snowflake with Kafka Connect</h3>
 
</div>

<!-- ABOUT THE PROJECT -->
## About The Project
This project demonstrates how to replicate data from a PostgreSQL database to Snowflake using the Debezium Connector and the Snowflake Sink Connector. The Debezium Connector captures data changes from the PostgreSQL database, and the Snowflake Sink Connector streams the changes to a Snowflake database.


[![cdc-with-debezium-kafka-drawio.png](https://i.postimg.cc/FHwxQpkF/cdc-with-debezium-kafka-drawio.png)](https://postimg.cc/yDXRmFT2)

## Built With
<br/>

* ![Postgres](https://img.shields.io/badge/PostgresQL-%23316192.svg?style=for-the-badge&logo=postgresql&logoColor=white)

* ![SnowfLake](https://img.shields.io/badge/snowflake-52b5f7.svg?style=for-the-badge&logo=snowflake&logoColor=white)

* ![Apache Kafka](https://img.shields.io/badge/Apache%20Kafka-000000?style=for-the-badge&logo=Apache%20Kafka&logoColor=white)


## Prerequisites
* A PostgreSQL database instance with a database and tables to replicate.
* A Snowflake account with the necessary access credentials.
* Java 8 or later installed on your machine.
* Apache Kafka installed on your machine.

## Setup
* Install the Debezium PostgreSQL connector by following the instructions in the [Debezium documentation](https://debezium.io/documentation/reference/1.5/connectors/postgresql.html).
* Install the Snowflake Sink Connector by following the instructions in the [Snowflake documentation](https://docs.snowflake.com/en/user-guide/kafka-connector-install).
* Configure the PostgreSQL database by setting the `wal_level parameter to logical` in the postgresql.conf file.
* Create a new user with replication privileges and set up a replication slot using the `pg_create_logical_replication_slot` function.
* Configure the Debezium Connector by setting the necessary parameters in the connector configuration file.
* Configure the Snowflake Sink Connector by setting the necessary parameters in the connector configuration file.
* Start the Kafka Connect service.
* Start the Debezium Connector and the Snowflake Sink Connector by submitting their configuration files to the Kafka Connect REST API using the curl command.

<!-- CONTACT -->
## Contact

[@ابراهيم انيس](https://twitter.com/ibrahim__Anees)


<p align="right">(<a href="#readme-top">back to top</a>)</p>


