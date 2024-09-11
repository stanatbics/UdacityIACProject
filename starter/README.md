# CD12352 - Infrastructure as Code Project Solution
# stan

## Spin up instructions
./main.sh create us-east-1 StanNetworkInfra network.yml network-parameters.json

./main.sh create us-east-1 StanAppInfra udagram.yml udagram-parameters.json

## Tear down instructions
Emptying s3 bucket
./main.sh delete us-east-1 StanAppInfra

./main.sh delete us-east-1 StanNetworkInfra

## Other considerations
- added diagram - infrastructure_diagram.png
- Deployed index.html as a static content using cloudfront - http://d1x4s4fyb468yw.cloudfront.net/
- Load Balancer Public URL - http://stanap-webap-txnajqprnktf-1079223550.us-east-1.elb.amazonaws.com/
