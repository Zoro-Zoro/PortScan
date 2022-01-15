##PortScanning🚪

```python
import socket

ip = raw_input('ip > ')

for port in range(65535):
	s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
	if s.connect_ex((ip, port)) == 0:
		print("PORTA > {} < ABERTA".format(port))
	else:
		print("PORTA > {} < FECHADA".format(port))
```
