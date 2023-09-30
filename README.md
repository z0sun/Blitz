# Blitz

## Scenario 
After receiving customer complaints regarding load times for GET request to Nike.com our client Nike requested a solution to the latency issue.

## Troubleshooting
- Within a test enviroment, 1000 request were made to the web server in order to record response time.
- The blitz results showed latency of around 40ms.

## Resolution
In order to resolve the latency issues the decision was made to add a CDN via CloudWatch. Having the webpage cached within the CDN improvded latency to 6ms by routing users to the CDN for static request. 

## Optimization 
Although implenting a CDN would be a the most resonable fix for this latency issue, to optimize latency results horizontal scaling with the additon of a load balancer could also remedy latency issues by routing high user traffic to new resources by way of the load balancer. 
