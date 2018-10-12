1.Move mfsc/ to ryu/app,move topo to mininet/custom.
2.Use "ryu-manager --observe-links monitor_switch_13.py" to start ryu.
3.Use "mn --switch ovsk,protocols=OpenFlow13 --controller=remote,ip=127.0.0.1,port=6633 --custom custom/topo.py --topo mytopo" to start mininet.
4.Use "pingall" twice.
5.Use "xterm h1 h2 h3..." to start hosts.
6.Use iperf to create flows among hosts.
7.You can the number of covered flows using per-flow,random-wildcard,D-FSC and G-FSC in controller.

