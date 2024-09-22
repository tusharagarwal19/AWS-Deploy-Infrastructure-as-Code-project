# CD12352 - Infrastructure as Code Project Solution
# Tushar Agarwal

## Spin up instructions
1. Open Visual Studio Code
2. Clone the branch at /workspace directory
3. Go to /workspace/AWS-Deploy-Infrastructure-as-Code-project-1/starter
4. To create the network stack, run the below command
    sh ./stack_scripts/create_stack.sh udagram-iac network.yml network-parameters.json
5. To create the Webapp stack, run the below command
    sh ./stack_scripts/create_stack.sh udagram-webapp udagram.yml udagram-parameters.json

Outputs
1. To verify the output of each stack, go to the Resources tab of both the stacks and verify the resources that are created.
2. Final output i.e. Udagram app can be checked at below URL. 
   http://gk-dem-webap-s4tlqovy08rd-2111062416.us-east-1.elb.amazonaws.com
3. Below is the screenshot of the udagram webapp:
   <img width="696" alt="image" src="https://github.com/user-attachments/assets/dd62bfdc-5845-446c-9c88-172ce65bb08a">


## Tear down instructions

1. Delete the stack using below command
   sh ./stack_scripts/delete_stack.sh udagram-webapp
2. Delete the network stack using below command
   sh ./stack_scripts/delete_stack.sh udagram-iac
