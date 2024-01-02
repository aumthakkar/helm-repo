This Repo consists of a Helm Chart consisting of all the components of a Voting App.  

It consists of the votingapp main folder which has the voting-app-deploy.yaml and voting-app-svc.yaml files in its templates folder

This repo has the deployments for:
- the postgres app,
- the redis app, 
- the result app & 
- the worker app.

All these respective deployments and its corresponding services are each configured as a sub-chart and are each configured  in the charts folder. 

The worker deployment doesn't need a service so in all there are 5 deployments and 4 services.

Once this repo is cloned to your machine, the entire app can be provisioned by issuing the - "helm install votingapp ." command from the directory where you have this repo cloned.

I have used nodePort type services for both, the Voting App and the Result App, so this can be tested on your own machine. The votingApp uses port 30001 and the resultApp uses on port 30002.
