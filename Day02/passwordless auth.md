In Passwordlees Authentication We need have Control Node( User pc) and Manage nodes (target server or vms)

Passwordlees Authentication  can be achieved by two ways
                                               1. SSH key
                                               2. Password
and also Ansible should be installed in Host Server(Control Node)

# to make passwordless auth we need to use ssh-keygen
# commands 
1. ssh-keygen in control-node server
2. copy public key of control-node
3. ssh-keygen in manage-node server
4. paste public key in authorized folder of manage node


ssh-copy-id -f "-o IdentityFile <PATH TO PEM FILE>" ubuntu@<INSTANCE-PUBLIC-IP>

ssh-copy-id -f "-o IdentityFile \Users\asus\Downloads\terra.pem" ubuntu@44.204.53.25


cp /mnt/c/Users/YourUsername/Downloads/ec2-key.pem ~/.ssh/ec2-key.pem
\Users\asus\Downloads\terra.pem
cp /mnt/c/Users/asus/Downloads/terra.pem ~/.ssh/terra.pem
cp \mnt\c\Users\asus\Downloads\terra.pem ~\.ssh\terra.pem

chmod 400 ~/.ssh/terra.pem
ssh -i ~/.ssh/terra.pem ubuntu@54.89.227.239

54.89.227.239
ssh-copy-id -f "-o IdentityFile /mnt/c/Users/asus/Downloads/terra.pem " ubuntu@54.89.227.239

 eval "$(ssh-agent -s)"
 $ ssh-add ~/.ssh/terra.pem
  ssh ubuntu@54.89.227.239

  ssh-copy-id -f "-o IdentityFile \Users\asus\Downloads\ec2key.pem" ubuntu@44.203.84.184

  ssh-copy-id -f "-o IdentityFile /mnt/c/Users/asus/Downloads/terra.pem" ubuntu@44.204.53.25
  ssh-copy-id -f "-o IdentityFile /mnt/c/Users/asus/Downloads/ec2key.pem" ubuntu@44.203.84.184

ssh-copy-id -i /mnt/c/Users/asus/Downloads/terra.pem
/identity_file ubuntu@44.203.84.184