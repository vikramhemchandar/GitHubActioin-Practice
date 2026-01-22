# GitHubActioin-Practice
A practical session on How to create a GitHub Actions pipeline and how go connect with EC2 instance. 

Here, I have written a simple index.html file and I will execute this on an Amazon EC2 instance.

### Steps to follow
- Create an EC2 instance with SSH, HTTP and HTTPS ports enabled
- Install nginx on EC2 instance
- Create Secret variable: Repository settings -> Secrets and Variables -> Actions -> New repository secret and add different variables
    - EC2_HOST: provide the public IP address
    - EC2_USERNAME: provide the username, here it is ubuntu
    - EC2_SSH_KEY: provide the SSH key from pem file
- I have used appleboy SSH and SCP actions to SCP the index file and SSH to copy the index file and copy to /var/www/html. For reference go to - https://github.com/appleboy
- At last, user public IP address of the EC2 and give it in your browser