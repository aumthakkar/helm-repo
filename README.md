This Repo consists of a Helm Chart consisting of all the components of a Voting App.  

It consists of the votingapp main folder which has the Voting App deployment and service.yaml files in its templates folder

Then it has the other deployments for:
-  the postgres app,
-  the redis app, 
- the result app & 
- the worker app

It also and all its corresponding services. 

Both these respective deployments and its corresponding services are in the charts folder each as a sub-chart. 

Please note that the worker deployment doesn't need a service so in all there are 5 deployments and 4 services.

