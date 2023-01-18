# lbgsimonapp
This Repo contains a copy of the example azure vote app source code
main.yaml can be used for a pipeline to:
  Containerise the application
  Push it to an eixsting ACR
  Fetch the latest image and deploy onto an existing AKS cluster
  
 Variables are passed in using vars.yaml.
 
 Improvements:
 due to time constraints this is not a complete solution and there are changes that can be made
  1. Creating image pull secret by fetching SP values from a key vault
  2. Specific artifact generation and selection
  3. Rolling deployment strategy to deploy another version via canary to test application
  4. Integration of AKS and ACR creation
