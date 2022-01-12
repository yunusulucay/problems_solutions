If you get an error like this. (You can not connect to mongodb)

```
● mongod.service - MongoDB Database Server
   Loaded: loaded (/lib/systemd/system/mongod.service; enabled; vendor preset: enabled)
   Active: failed (Result: exit-code) since Wed 2020-02-19 22:39:00 CET; 2s ago
     Docs: https://docs.mongodb.org/manual
  Process: 29368 ExecStart=/usr/bin/mongod --config /etc/mongod.conf (code=exited, status=14)
 Main PID: 29368 (code=exited, status=14)

Feb 19 22:39:00 pop-os systemd[1]: Started MongoDB Database Server.
Feb 19 22:39:00 pop-os systemd[1]: mongod.service: Main process exited, code=exited, status=14/n/a
Feb 19 22:39:00 pop-os systemd[1]: mongod.service: Failed with result 'exit-code'.
```

Implement these ->

$ sudo rm -rf /tmp/mongodb-27017.sock

$ sudo service mongod start
