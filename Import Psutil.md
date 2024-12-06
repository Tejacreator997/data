python:

import psutil(python system and process utilities)

#list of servers hostname or IP address 
servers_list = ["server1","server2","server3","server4"] 

#to check cpu utilization on each server in server_list

def check_cpu_usage(server:name):         
   cpu_usage = psutil.cpu_percent(interval=1)
   return cpu_usage

#function to find server with high cpu
def find_high_cpu_servers(server_list,threshold=85):
high_cpu_server = []

  for server in server list:
  cpu_usage = check_cpu_usage (server)
  if cpu_usage > threshold:
  print("Warning: (server) has high cpu at (cpu_usage)%" s1 -45 s2-55 s3-65  s4-75
  high_cpu_server.append(server)

  else:
  print ("information: (server) CPU usage is normal at (cpu_usage)%")

  return high_cpu_server  