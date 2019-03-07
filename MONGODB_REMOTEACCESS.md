- By default, MongoDB is listening on 127.0.0.1:27017 only:

'''
$ sudo netstat -tnlp
'''

'''
Proto Recv-Q Send-Q Local Address   Foreign Address State  PID/Program name
tcp        0      0 127.0.0.1:27017 0.0.0.0:*       LISTEN 1106/mongod
'''


- Open MongoDB configuration file /etc/mongod.conf and change bindIp by adding required LAN interfaces or configure it to bind to all interfaces, for example:
'''
# network interfaces
net:
  port: 27017
  bindIp: 127.0.0.1,192.168.0.100 # Enter 0.0.0.0,:: to bind to all interfaces
'''

Restart mongod to apply modifications:

'''
$ sudo service mongod restart
'''


- Now mongod is listening on configured interfaces and can be accessible remotely:

'''
$ sudo netstat -tnlp
Proto Recv-Q Send-Q Local Address       Foreign Address State  PID/Program name
tcp        0      0 127.0.0.1:27017     0.0.0.0:*       LISTEN 19757/mongod
tcp        0      0 192.168.0.100:27017 0.0.0.0:*       LISTEN 19757/mongod
'''
