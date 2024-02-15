# Scale It!
* Create autoscale group that will contain one ondemand instance and will scale on spot instances.
* Set up scaling policy based on AVG CPU usage
* Set up scaling policy based on requests amount that allows non-linear growth

## Launch Template Configuration
![lt.png](screenshots%2Flt.png)
## Autoscaling Group Configuration
![ag-details.png](screenshots%2Fag-details.png)
![ag-lt.png](screenshots%2Fag-lt.png)
![ag-instance_type.png](screenshots%2Fag-instance_type.png)
![ag-lb.png](screenshots%2Fag-lb.png)
![ag-advanced.png](screenshots%2Fag-advanced.png)
### Spot configuration
![ag-spot.png](screenshots%2Fag-spot.png)
### Scaling configuration
![ag-scaling.png](screenshots%2Fag-scaling.png)
## Testing

Run Siege command:
```shell
siege -c250 -t60s -d3 http://hla-autoscaling-lb-1-255556812.eu-north-1.elb.amazonaws.com
```

![img.png](screenshots%2Fimg.png)

![ec2-spot.png](screenshots%2Fec2-spot.png)

![activity-history.png](screenshots%2Factivity-history.png)




