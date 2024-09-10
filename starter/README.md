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
- Deployed index.html as a static content using cloudfront - https://d1wljpz4ytafgq.cloudfront.net/
- Load Balancer Public URL - http://stanap-webap-2gjqfsa5b6tv-1166497746.us-east-1.elb.amazonaws.com/
