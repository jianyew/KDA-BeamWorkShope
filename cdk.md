### CDK 部署



下载 [CDK](https://github.com/jianyew/amazon-kinesis-analytics-beam-taxi-consumer/tree/master/cdk)，从 github

![image-20201123131143154](/Users/wjianye/Desktop/BeamOnKDA/image/image-20201123131143154.png)























CMD

java -jar /Users/wjianye/kspace/repo/amazon-kinesis-replay/target/amazon-kinesis-replay-1.0-SNAPSHOT.jar -streamRegion cn-north-1 -streamName beam-workshop -objectPrefix artifacts/kinesis-analytics-taxi-consumer/taxi-trips-partitioned.json.lz4/dropoff_year=2018/ -speedup 720



java -jar amazon-kinesis-replay-1.0-SNAPSHOT.jar -streamRegion cn-north-1 -streamName beam-workshop -bucketRegion cn-north-1 -objectPrefix artifacts/kinesis-analytics-taxi-consumer/taxi-trips-partitioned.json.lz4/dropoff_year=2018/ -speedup 720




 export AWS_PROFILE="bjs"

 aws-bigdata-blog



aws s3 sync s3://aws-bigdata-blog/artifacts/kinesis-analytics-taxi-consumer/taxi-trips-partitioned.json.lz4/ .  --profile default