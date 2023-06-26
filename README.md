# Mikrotik
<img src='https://i.imgur.com/YS4p1JS.png'>
Comandos e soluções mikrotik

**Limitar a quantidade de conexões(Portas) para os GATO NET**
```
/ip firewall filter
add action=drop chain=forward connection-limit=400,32 protocol=tcp src-address=\
    172.254.255.0/29 tcp-flags=syn
```
**Limitamos a 400 portas**
