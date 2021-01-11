Adout:
This roles enables you to create systemd timers which call scripts or execute commands.
For bash script (monitoring psql script to postgres database)
Start script from /home/user/script.sh with database connection string /monitoring.conf:q

Exemple:

 Edit monitoring.j2 template
ipPostgresServer:port:database:user:password

 Edit vars:
Name Service:
   Name Service:
     user: user
     group: group
     script: script

     
Usage:
1. Edit monitoring.j2
2. Edit vars
3. Upload service file
4. Upload timer file
5. copy monitoring file to home directory (with database connection string)
6. Enable timer
