# data-eng-quest
Manifest for DATA engineering quest.


Technical task for Data Engineer Position

All your tasks should be completed using docker image. You will analyse and prepare insights
for water quality open data set.
Go to [https://hub.docker.com/] and choose any Docker image containing Apache Kafka and run
it.
Follow the steps below:
1. Create new Kafka topic called: seb-demo
2. Download latest Apache Spark version.
3. Create folder for initial data. (eg. /opt/data/initial)
4. Please download the data set &quot;Waterbase-Water Quality (CSV files)&quot; into the folder from
previous step. [https://data.europa.eu/euodp/en/data/dataset/DAT-163-en]
5. Unzip recently downloaded file. You will be working with dataset:
Waterbase_v2018_1_T_WISE4_AggregatedData.csv
6. Create target folder (eg. /opt/data/target) which you will use for file conversion (CSV to
Parquet or CSV to Avro).
7. Convert dataset using Apache Spark to parquet or to avro format and store it in target
location (eg. /opt/data/initial -&gt; Spark -&gt; /opt/data/target)
8. Create structured streaming script or application using Apache Spark following these rules:
 Use target file as input [ref: step 7]
 Proceed with data aggregations, data cleansing, or similar to analyse the data by
country.
 Publish the analysis results to the Kafka topic seb-demo
9. Ensure that streaming pipeline is working. This will be required during the exercise review.
Bonus:
10. Create subscription in Kafka for seb-demo topic.
11. Show the outcome in BI or any other data visualization / data analysis tool.
12. Create automation for your solution with ansible, jenkins, git actions or similar.
13. Prepare and apply testing strategy.
NOTE: Please do not make this document or the results of this task public. If you are using
github please create it as private project.