# GitHubActioin-Practice
GitHub Actions pipeline practice

### Steps to follow
- Create an EC2 instance with SSH, HTTP and HTTPS ports open
- Install nginx on EC2 instance
- Create Secret variable: Repository settings -> Secrets and Variables -> Actions -> New repository secret and add different variables
    - EC2_HOST: <IP Address>
    - EC2_USERNAME: <username> //here it is ubuntu
    - EC2_SSH_KEY: <SSH KEY> //pem file key
- I have used appleboy SSH and SCP actions here. For reference go to - https://github.com/appleboy