Useful cron jobs:

0 23    * * *   root    shutdown -h now #shut down PC daily at 23:00
0 17    * * *   root bash -c 'for i in /home/enumtheworld/Downloads/*.{pdf,docx,png,jpg,PDF,DOCX}; do shred -zvu "$i" -n20; done' # shred all documents in /Downloads folder

Logs are saved here:
sudo vim /var/log/syslog

Errors and responses are saved here:
sudo tail /var/mail/root

When executing a specific file, do not forget to chmod+x it
