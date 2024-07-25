
==> ShellScript is used for only Linux
==> It is little complex compare to Ansible
==> Ansible is Idempotence in nature(run onces or multiple times but impact is onces) 
==> ShellScript changes

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