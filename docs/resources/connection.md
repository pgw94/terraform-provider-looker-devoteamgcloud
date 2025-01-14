---
page_title: "looker_connection Resource - terraform-provider-looker"
subcategory: ""
description: |-
  
---
# looker_connection (Resource)

## Example Usage
```terraform
resource "looker_connection" "example" {
  name            = "testdummy901"
  username        = "hegdgxme"
  database        = "hegdgxme"
  dialect_name    = "postgres"
  port            = "5432"
  host            = "surus.db.elephantsql.com"
  password        = "polite-sculpin"
  ssl             = true
  max_connections = 5
}
```

## Example Output
```terraform
# looker_connection.example:
resource "looker_connection" "example" {
  database        = "hegdgxme"
  dialect_name    = "postgres"
  host            = "surus.db.elephantsql.com"
  id              = "testdummy901"
  max_connections = 5
  name            = "testdummy901"
# password        = (sensitive value)
  port            = "5432"
  ssl             = true
  username        = "hegdgxme"
}
```

<!-- schema generated by tfplugindocs -->
## Schema

### Required

- `dialect_name` (String) <table>
<thead>
<tr>
<th>name</th>
<th>dialect_name</th>
</tr>
</thead>
<tbody>
<tr>
<td>Actian Avalanche</td>
<td>actian_avalanche</td>
</tr>
<tr>
<td>Amazon Athena</td>
<td>athena</td>
</tr>
<tr>
<td>Amazon Aurora MySQL</td>
<td>amazonaurora</td>
</tr>
<tr>
<td>Amazon Redshift</td>
<td>redshift</td>
</tr>
<tr>
<td>Apache Druid</td>
<td>druid</td>
</tr>
<tr>
<td>Apache Druid 0.13+</td>
<td>druid_13</td>
</tr>
<tr>
<td>Apache Druid 0.18+</td>
<td>druid_18</td>
</tr>
<tr>
<td>Apache Hive 2</td>
<td>hive2</td>
</tr>
<tr>
<td>Apache Hive 2.3+</td>
<td>hive2_3</td>
</tr>
<tr>
<td>Apache Hive 3.1.2+</td>
<td>hive3</td>
</tr>
<tr>
<td>Apache Spark 1.5+</td>
<td>spark1_5</td>
</tr>
<tr>
<td>Apache Spark 2.0</td>
<td>spark2_0</td>
</tr>
<tr>
<td>Apache Spark 3+</td>
<td>spark_3</td>
</tr>
<tr>
<td>ClickHouse</td>
<td>clickhouse</td>
</tr>
<tr>
<td>Cloudera Impala</td>
<td>impala</td>
</tr>
<tr>
<td>Cloudera Impala 3.1+</td>
<td>impala_3_1</td>
</tr>
<tr>
<td>Cloudera Impala 3.1+ with Native Driver</td>
<td>impala_native_3_1</td>
</tr>
<tr>
<td>Cloudera Impala with Native Driver</td>
<td>impala_native</td>
</tr>
<tr>
<td>Clustrix</td>
<td>clustrix</td>
</tr>
<tr>
<td>DataVirtuality</td>
<td>datavirtuality</td>
</tr>
<tr>
<td>Databricks</td>
<td>databricks</td>
</tr>
<tr>
<td>Denodo</td>
<td>denodo</td>
</tr>
<tr>
<td>Denodo 7</td>
<td>denodo7</td>
</tr>
<tr>
<td>Denodo 8</td>
<td>denodo8</td>
</tr>
<tr>
<td>Dremio</td>
<td>dremio</td>
</tr>
<tr>
<td>Dremio 11+</td>
<td>dremio_11</td>
</tr>
<tr>
<td>Exasol</td>
<td>exasol</td>
</tr>
<tr>
<td>Firebolt</td>
<td>firebolt</td>
</tr>
<tr>
<td>Google BigQuery Legacy SQL</td>
<td>bigquery</td>
</tr>
<tr>
<td>Google BigQuery Standard SQL</td>
<td>bigquery_standard_sql</td>
</tr>
<tr>
<td>Google Cloud PostgreSQL</td>
<td>google_cloud_postgres</td>
</tr>
<tr>
<td>Google Cloud SQL</td>
<td>googlecloudsql</td>
</tr>
<tr>
<td>Google Cloud Spanner</td>
<td>spanner</td>
</tr>
<tr>
<td>Greenplum</td>
<td>greenplum</td>
</tr>
<tr>
<td>IBM DB2</td>
<td>db2</td>
</tr>
<tr>
<td>IBM DB2 for AS400 and System i</td>
<td>as400</td>
</tr>
<tr>
<td>IBM Netezza</td>
<td>netezza</td>
</tr>
<tr>
<td>MariaDB</td>
<td>mariadb</td>
</tr>
<tr>
<td>Microsoft Azure PostgreSQL</td>
<td>azure_postgres</td>
</tr>
<tr>
<td>Microsoft Azure SQL Database</td>
<td>msazuresql</td>
</tr>
<tr>
<td>Microsoft Azure Synapse Analytics</td>
<td>mssqldw</td>
</tr>
<tr>
<td>Microsoft SQL Server 2008+</td>
<td>mssql_2008</td>
</tr>
<tr>
<td>Microsoft SQL Server 2012+</td>
<td>mssql_2012</td>
</tr>
<tr>
<td>Microsoft SQL Server 2016</td>
<td>mssql_2016</td>
</tr>
<tr>
<td>Microsoft SQL Server 2017+</td>
<td>mssql_2017</td>
</tr>
<tr>
<td>MongoBI</td>
<td>mongobi</td>
</tr>
<tr>
<td>MySQL</td>
<td>mysql</td>
</tr>
<tr>
<td>MySQL 8.0.12+</td>
<td>mysql_8</td>
</tr>
<tr>
<td>Oracle</td>
<td>oracle</td>
</tr>
<tr>
<td>Oracle ADWC</td>
<td>oracle_dwcs</td>
</tr>
<tr>
<td>PostgreSQL 9.5+</td>
<td>postgres</td>
</tr>
<tr>
<td>PostgreSQL pre-9.5</td>
<td>postgres9_1</td>
</tr>
<tr>
<td>PrestoDB</td>
<td>presto</td>
</tr>
<tr>
<td>PrestoSQL</td>
<td>prestosql</td>
</tr>
<tr>
<td>Qubole Presto</td>
<td>qubole_presto</td>
</tr>
<tr>
<td>SAP HANA</td>
<td>hana</td>
</tr>
<tr>
<td>SAP HANA 2+</td>
<td>hana_2</td>
</tr>
<tr>
<td>SingleStore</td>
<td>memsql</td>
</tr>
<tr>
<td>SingleStore 7+</td>
<td>memsql_7</td>
</tr>
<tr>
<td>Snowflake</td>
<td>snowflake</td>
</tr>
<tr>
<td>Teradata</td>
<td>teradata</td>
</tr>
<tr>
<td>Trino</td>
<td>trino</td>
</tr>
<tr>
<td>Vector</td>
<td>vector</td>
</tr>
<tr>
<td>Vertica</td>
<td>vertica</td>
</tr>
</tbody>
</table>
- `name` (String) Name of the connection. Also used as the unique identifier

### Optional

- `after_connect_statements` (String)
- `always_retry_failed_builds` (Boolean)
- `certificate` (String, Sensitive)
- `cost_estimate_enabled` (Boolean)
- `database` (String)
- `db_timezone` (String)
- `disable_context_comment` (Boolean)
- `file_type` (String)
- `host` (String)
- `jdbc_additional_params` (String)
- `maintenance_cron` (String)
- `max_billing_gigabytes` (String)
- `max_connections` (Number)
- `oauth_application_id` (String)
- `password` (String, Sensitive)
- `pdt_api_control_enabled` (Boolean)
- `pdt_concurrency` (Number)
- `pool_timeout` (Number)
- `port` (String)
- `query_timezone` (String)
- `schema` (String)
- `sql_runner_precache_tables` (Boolean)
- `sql_writing_with_info_schema` (Boolean)
- `ssl` (Boolean)
- `tmp_db_name` (String)
- `tunnel_id` (String)
- `user_db_credentials` (Boolean)
- `username` (String)
- `verify_ssl` (Boolean)

### Read-Only

- `id` (String) The ID of this resource.
