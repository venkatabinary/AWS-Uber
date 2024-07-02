# AWS-Uber
AWS Uber

https://www.uber.com/blog/streaming-real-time-analytics/ <br>
We performed trials in a local machine with individual components, simulating data inflow with a copy of data from S3. We built components for ingestion, Redis, and visualization in docker containers, wrote a script to trigger post messages to the ingestion container to simulate object creation events, and developed ingestion code to read, filter, transform, and insert events into Redis. We initially chose Grafana for visualization to quickly test the flow of data from source to a live graph. This was successful, so we replaced Grafana with a Python Dash container to build dynamic visualization for one of our use cases. With corresponding components in AWS, we came up with the below architecture.
<br>

![image](https://github.com/venkatabinary/AWS-Uber/assets/96198186/f486fc9e-db97-41e7-9293-3c95831c04bb)
