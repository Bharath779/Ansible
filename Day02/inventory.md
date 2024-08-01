need to create inventory.ini and we can store manage nodes there like server 
if you don't want to use inventory.ini you can use /etc/ansible/host
syntax is-- 
#          ansible -i inventory.ini -m ping all
#          ansible -i inventory.ini -m shell -a "mkdir folder all"
        