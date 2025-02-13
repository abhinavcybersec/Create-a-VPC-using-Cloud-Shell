# Create a Virtual Private Cloud
## Tasks
- Conducting research to explore the security of the configuration settings of the new cloud network setup.

## Setup
- Logging in to the account provided by QuickLabs
- Activating Cloud Shell
- Following the steps to complete the task

## Steps
### Listing the Active Account name
> gcloud auth list

![alt text](image.png)

### Listing the Project ID
> gcloud config list project

![alt text](image-1.png)

### Creating a Network
> gcloud compute networks create labnet --subnet-mode=custom

![alt text](image-2.png)

### Creating a Subnet
> gcloud compute networks subnets create labnet-sub \
>       --network labnet \
>       --region europe-west1 \ 
>       --range 10.0.0.0/28

![alt text](image-3.png)

### View Networks
> gcloud compute networks list

![alt text](image-4.png)

### List Subnets
> gcloud compute networks subnets list --network=labnet

![alt text](image-5.png)

### Conclusion
Now I am confident in using Cloud Shell and creating a Virtual Private Cloud, along with setting up the subnets.