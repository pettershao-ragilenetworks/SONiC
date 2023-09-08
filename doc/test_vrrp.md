Example:-
```
admin@sonic:~$ redis-cli -n 4 HGETALL " VRRP|Vlan10|10"

1) "vip"
2) "4.1.1.100/24,4.1.1.200/24,2000::50/64"
3) "priority"
4) "100"
5) "adv_interval"
6) "1000"
7) "admin_status"
8) "up"
9) "version"
10)"3"
11)"preempt"
12)"enabled"
13)"track_interface"
14)"Ethernet5, Ethernet9"
15)"priority_decrement"
16)"20"
```



Example:-
```
admin@sonic:~$ redis-cli -n 0 HGETALL "INTF_TABLE:Vrrp4-5"
1) "vmac"
2) "00:00:5e:00:01:05"
3) "oper_state"
4) "up"
```
```
admin@sonic:~$ redis-cli -n 0 HGETALL "INTF_TABLE:Vrrp4-5:10.10.10.1/32"
1) "NULL"
2) "NULL"
```
