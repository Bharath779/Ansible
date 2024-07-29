# create a new repository on the command line
echo "# apache-httpd" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/Bharath779/apache-httpd.git
git push -u origin main

# push an existing repository from the command line
git remote add origin https://github.com/Bharath779/apache-httpd.git
git branch -M main
git push -u origin main

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

# Important commands of Ansible

# ad-hoc command
1. ansible all<Host> -i inventory.ini -m <module_name> -a <argument_name>

# playbook command
2. ansible-playbook -i inventory.ini <File_name>

# roles command
# To initialize roles
1. ansible-galaxy role init <role_name>