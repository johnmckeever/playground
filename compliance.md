# MettleCI Cloud Pak Compliance Rule Reference \nThis page lists the example Compliance Rules supplied with MettleCI for IBM Cloud Pak for Data. \nEach Compliance Rule is supplied as a `.groovy` file which makes use of the MettleCI-enhanced Gremlin graph query [DSL](https://en.wikipedia.org/wiki/Domain-specific_language). \n| --------- | ----------- | \n| Rule name | Description | \n| --------- | ----------- | \n| [Adjacent Transformers](Adjacent Transformers.md) | Identifies flow designs with adjacent Transformer stages. | \n| [Aggregator Stage Not Preceded by Check Sort Stage](Aggregator Stage Not Preceded by Check Sort Stage.md) | Aggregator Stage will only return the correct result if the keys are pre-sorted | \n| [Audit Annotation](Audit Annotation.md) | Identifies where sensitive information may potentially be present in DataStage Job and Sequence Annotations. | \n| [compliance](compliance.md) |  | \n| [Connection Contains Parameter References](Connection Contains Parameter References.md) | Identifies Connections created by the migration from legacy Datastage to NextGen that contain references to | \n| [Connection Not Using Secrets Vault](Connection Not Using Secrets Vault.md) | Identifies Connections that do not store their credentials to use secrets in a vault. | \n| [Database Query From File](Database Query From File.md) | Ensures if Database Connectors and Stages reads SQL statement from file. | \n| [Database Row Limit](Database Row Limit.md) | Identifies Connectors Stages with a configured Database Row Limit. | \n| [DataSet Not Using Same Partition](DataSet Not Using Same Partition.md) | Identifies Data Sets not using the 'Same' partitioning method | \n| [Date Format in Annotation](Date Format in Annotation.md) | Identify whether the a Flow annotation contains instances of particular arbitrary text.  This example rule looks for dates. | \n| [DB2 with No Non Recovery Load](DB2 with No Non Recovery Load.md) | Identify Db2 Stages using bulk load with Non Recovery Load set to 'No'. | \n| [DB Connector Not Auto Generate SQL](DB Connector Not Auto Generate SQL.md) | Identifies Connections that do not use Auto Generate SQL. | \n| [DB Tables Referenced Are Fully Qualified](DB Tables Referenced Are Fully Qualified.md) | Identifies where database table references are not fully-qualified. | \n| [Debug Row Limit](Debug Row Limit.md) | Identifies row limits in debug stages (Peek, Sample, Tail) | \n| [Default Naming](Default Naming.md) | Default Stage Names for Parallel Jobs, Server Jobs, and Job Sequences | \n| [Duplicate File References](Duplicate File References.md) | Verifies that a sequential file is... | \n| [Duplicate Stage Names](Duplicate Stage Names.md) | Detect duplicate Stage names in a job. | \n| [File Reference Missing Required Parameter](File Reference Missing Required Parameter.md) | Ensures that all File Stages must use variables for determining paths | \n| [File Row Limit](File Row Limit.md) | Identifies row limits in file-based stages (Sequential File, Complex Flat File). | \n| [Flow Naming](Flow Naming.md) | Checks the Flow name against a list of known prohibited name patterns. | \n| [Flow Parameter Missing Default Value](Flow Parameter Missing Default Value.md) | Identify flow parameters within a default value. | \n| [Flow Parameter Naming](Flow Parameter Naming.md) | Identifies where naming standards for Flow Parameters and Parameter Sets are breached. | \n| [Flow Parameter Not In A Parameter Set](Flow Parameter Not In A Parameter Set.md) | Identify Flow Parameters that are not in a Parameter Set. | \n| [Flow Using Random Function](Flow Using Random Function.md) | Identify Transformers (or other stages) using Random functions which produce non-deterministic output. | \n| [Flow Using Transformer Surrogate Key](Flow Using Transformer Surrogate Key.md) | Identifies flow designs that use NextSurrogateKey() in a Transformer. | \n| [Hardcoded DB Credentials](Hardcoded DB Credentials.md) | Ensures that all Database Connectors must use variables for location and credentials | \n| [Hardcoded File Paths](Hardcoded File Paths.md) | Ensures that all File Stages must use variables for determining paths | \n| [Join Partition vs Join Key](Join Partition vs Join Key.md) | Reports Join stages where the join key does not match the partitioning of the input links. | \n| [Link Sort](Link Sort.md) | Identifies link sorts. | \n| [Log Column Values](Log Column Values.md) | Identify Stages configured to Log column values on first row error | \n| [Lookup Failure](Lookup Failure.md) | Identifies Lookup Stages with Lookup set to Fail. | \n| [One Dataflow](One Dataflow.md) | Verifies that there is only one data flow in a DataStage Flow. | \n| [Oracle Connector Not Using Partitioned Read](Oracle Connector Not Using Partitioned Read.md) | Identify Oracle Stages not configured to use partitioned reads. | \n| [Password Parameter Type Not Encrypted](Password Parameter Type Not Encrypted.md) | Flow parameters with names that suggest they will be used for supplying passwords should be set to use the type "Encrypted". | \n| [Prohibited Stages](Prohibited Stages.md) | Verifies that a job does not contain one or more prohibited stages. | \n| [Range Lookup Incorrectly Configured](Range Lookup Incorrectly Configured.md) | Checks that range lookups are correctly configured. | \n| [Redundant Sort](Redundant Sort.md) | Identifies unnecessary sort opertions witihn Job designs. | \n| [Schema Files](Schema Files.md) | Detect use of Schema Files. | \n| [Select All in Custom SQL](Select All in Custom SQL.md) | Identifies where "select *" syntax has been used in custom SQL code in database Connectors. | \n| [Sequential File Read Using Same Partitioning](Sequential File Read Using Same Partitioning.md) | Avoid reading from Sequential Files using the 'Same' partitioning method. | \n| [Sequential File With Reject Mode Not Set To Fail](Sequential File With Reject Mode Not Set To Fail.md) | Identifies Sequential Files with a Reject Mode not set to fail | \n| [Sort Post Join Stage](Sort Post Join Stage.md) | Identifies potentially redundant sorting (a sort stage or link sort) situated immediately after a Join stage | \n| [SQL in DB Connectors](SQL in DB Connectors.md) | Ensures that all DB Connectors not using SQL Statement to filter source data | \n| [Stage Naming](Stage Naming.md) | Stage naming standards for DataStage flows and watson pipelines. | \n| [System Time Dependency](System Time Dependency.md) | Identifies the use of system time functions in the job | \n| [Too Many Stages](Too Many Stages.md) | Identify whether a flow has too many stages. | \n| [Transformer Uses Abort After Rows](Transformer Uses Abort After Rows.md) | Detect an 'Abort after rows' greater than 0 setting in a Parallel Transformer. | \n| [Transformer With Unreferenced Stage Variable](Transformer With Unreferenced Stage Variable.md) | Identifies Transformer Stage with an unreferenced Stage Variable (including Loop Variables). | \n| [Unencrypted DB Passwords](Unencrypted DB Passwords.md) | Ensures that all Connectors must use encrypted Passwords | \n| [Unique Sort](Unique Sort.md) | Identifies unique sorts. | \n| --------- | ----------- | \n Page generated on Wed Dec 13 15:17:26 AEDT 2023 \n &copy; 2023 Data Migrators Pty Ltd \n [www.datamigrators.com](http://www.datamigrators.com)