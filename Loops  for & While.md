Loops : for & while

for: Iterates over a sequence (list,tuple or range)
while : Repeats as long as specified condition is "True"

Ex:for loop:

Need to monitor CPU usage across  a list of server .We can use a list of server name of IP address

python:

import psutill

#list of server names or IP
server = ["192.168.1.10" , "192.168.1.11",  "192.168.1.12"]

#Function to simulate CPU check
def check cpu(server):
    cpu_usage = psutil.cpu_percent(interval=1)
	print("f:server:(server)- CPU usage:(cpu_usage)%")
      
	  
	  
#Iterates over the list of server
for server in servers:
    check_cpu(server)
	
Ex-1: for loop: Tuple

Restart  a set of services on a server

import subprocess

#Tuple of services that needs to be restarted

services = ("nginx","docker","redis")

#Function to restart a service
def restart_service(services):
    print(f:Restarting (services)):
	result = subprocess.run(["sudo",systemctl",restart",service],capture_output=True ,text =True)
    print(f:"(service) restarted sucessfully")
	
  else:
  print(f:failed to/restart (service)")
  print(f"(services) restart failed")
  
  
#Iterate over the list of servers
for service in services:
    restart_service(services)

Ex-3: for loop:Tuple

you might need to deploy a specific  version range of an application  (1.0 to 1.5)
for version in range(10,16):
deployment_version=f"1.{version}"

1.10
1.11
1.12
1.13
1.14
1.15
1.16

	