# Approach from data collection to cloud platform and visualisation
> An AWS Lambda function gets triggered and inserts IoT data into an InfluxDB database instance which is used to develop dashboards with Grafana. An additional option is represented to trigger Lambda Step Functions to aggregate the data at particular time intervals (such as average at 5 minute intervals) and to insert the aggregated data into InfluxDB. The InfluxDB data can also be exported as CSV files into Amazon S3 buckets and be the data source to perform anomaly detection or other ML modeling with Amazon SageMaker.
![i](https://d2908q01vomqb2.cloudfront.net/f6e1126cedebf23e1463aee73f9df08783640400/2020/01/24/GrafanaBlogArchitecture.png)

* Set up InfluxDB and Grafana on your own Amazon EC2 instances.
* Set up AWS IoT Core resources and AWS Lambda function needed to populate the time series database.
* Develop Grafana dashboard(s) with real-time visualizations to track IoT data.