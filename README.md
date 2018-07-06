# boto-ec2

```
import boto3
region = 'us-east-1'
client = boto3.client('ec2', region_name=region )
response = client.describe_instances()
for reservation in response["Reservations"]:
        for instance in reservation["Instances"]:
print (instance["InstanceId"])
```
