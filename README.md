# Deploy-AWS-EC2-Instance-hosted-Linux-and-Windows-AMI

![aws8](https://user-images.githubusercontent.com/47071968/229265324-a182825f-614a-47a4-b02f-ab3a0f65e53a.png)

## Goal

launch Linux and Windows based EC2 Instances in us-east-1 region

## Pre-Requisites

    AWS Free Tier Account
    
    
## Deployment

    1. Create AWS EC2 Keypair in .pem format
    2. Create Linux EC2 Instance with below configuration
        a. Root volume of 10GB
        b. Instance Type: t2.micro
        c. Amazon Linux 2 AMI
        d. Attach Key Pair created in step 1
        e. Create and Attach Elastic IP
        
   3. Create Windows EC2 Instance with below configuration
        
        a. Root volume of 30 GB
        
        b. Instance Type: t2.micro
        
        c. Windows Server 2019 base
        
        d. Attach Key Pair created in step 1
        
        e. Create and Attach Elastic IP
        
    4. Calculate estimated billing for both instances created in previous steps and add pricing matrix in the comments box.
    
   ## Validation

NOTE: You may need to convert the keys from .pem to .ppk if you are using putty to connect to the Linux EC2. Follow the this This site was built using [LINK](https://devopsrealtime.com/how-to-convert-an-aws-keypair-from-pem-into-a-ppk-and-vice-versa/) to know how to convert the key format.

   1. Login to Linux EC2 Instance with default user name. Post in the comments the default user names of your favorite Linux flavored OS.
   2. Login to Windows EC2 Instance and confirm the Login status in the comments box.
   

   ## Destroy
   
    1. Terminate Both EC2 instances  to abide the Free Tier Limitations.
    2. Release the Elastic IP

If not confident, repeat the steps again. Good Luck.


