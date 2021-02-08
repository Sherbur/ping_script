# ping_script
import os
import sys

hostnames = [
    '10.10.1.1',
    '10.20.1.1',
    '10.30.1.1',
]

for hostname in hostnames:
    response = os.system('ping ' + hostname)
    if response == 0:
        print('\n' + hostname + ' is up')
    else:
        print('\n' + hostname + ' is down')
