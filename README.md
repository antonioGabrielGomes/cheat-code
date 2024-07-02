# ports

## 1. `netstat`

netstat is a network tool that can be used to check network connections, routing tables, interface statistics, masquerade connections, and multicast memberships.

### Comando

```sh
netstat -tuln
```
Parameters

    -t: Display TCP connections
    -u: Display UDP connections
    -l: Show only listening ports
    -n: Show port numbers instead of names

## 2. `ss`

ss (socket statistics) is a tool that can replace netstat. It can provide detailed statistics about network connections.

### Comando

```sh
ss -tuln
```

Parameters

    -t: Display TCP connections
    -u: Display UDP connections
    -l: Show only listening ports
    -n: Show port numbers instead of names

## 3. `lsof`

lsof (list open files) is a tool that lists information about open files, including network ports.

### Comando 

```sh
sudo lsof -i -P -n | grep LISTEN
```

Parameters

    -i: Selects listing of network-related open files
    -P: Show port numbers instead of service names
    -n: Show numerical addresses instead of resolving to names

## 4. `nmap`

nmap (Network Mapper) is an open-source tool for network exploration and security auditing. It can be used to check which ports are open on a specific host.

### Comando

To check open ports locally:
```sh
sudo nmap -sT -O localhost
```

Parameters

    -sT: Perform a full TCP connection scan
    -O: Detect the operating system

