# openhab-python-broadlink-doc
Documentation for integrating python-broadlink with openhab


## References
1. [python-broadlink repo](https://github.com/mjg59/python-broadlink)
2. [openhab - how to use python-broadlink](https://community.openhab.org/t/broadlink-bestcon-rm4c-mini-mqtt-openhab-on-raspberry-pi-3b/98268)
    
    
## Comments
1. [openhab - how to use python-broadlink](https://community.openhab.org/t/broadlink-bestcon-rm4c-mini-mqtt-openhab-on-raspberry-pi-3b/98268)
    1. In the OP, I followed the **Setup** section up to **Check connection** section
    2. When you run the discovery cli, make sure to note the device info returned, for example:
        1. 0x62be 192.168.1.120 a57c4fa7df24
2. Add Broadlink Map [mini_split.map](https://github.com/lems111/openhab-python-broadlink-doc/blob/master/mini_split.map)
3. Add Broadlink Items [broadlink.items](https://github.com/lems111/openhab-python-broadlink-doc/blob/master/broadlink.items)
4. Add Broadlink Rules [broadlink.rules](https://github.com/lems111/openhab-python-broadlink-doc/blob/master/broadlink.rules)
5. Add AC Control in Sitemap [default.sitemap](https://github.com/lems111/openhab-python-broadlink-doc/blob/master/default.sitemap)



## Tips
### Python-broadlink cli tips
1. [CLI READ ME](https://github.com/mjg59/python-broadlink/tree/master/cli)

2. Learn command
```
cd python-broadlink-master\cli
python broadlink_cli --device "0x5f36 10.0.0.42 24dfa7dee9ca" --learn
```

3. Send command
```
cd python-broadlink-master\cli
python broadlink_cli --device "0x5f36 10.0.0.42 24dfa7dee9ca" --send 2600060164380c0f0c100c2a0c100b2b0c0f0c100c100b2b0c2a0c100c0f0c100c2a0c2a0c100c100b100c100c0f0c100c0f0c100c100b100c100b100c100c2a0c100b100c100c0f0c100c0f0c100c2a0c100c0f0c100c100b2b0c2a0c2b0b2b0b2b0c2a0c2a0c2b0c0f0c100c2a0c100b100c100c0f0c100c100b100c100b2b0c2a0c100c0f0c100c0f0c100c100b2b0c0f0c2b0c0f0c100c2a0c100c0f0c100c0f0c100c100b100c100b100c100c0f0c100c100b100c100b100c100c0f0c100c100b100c100b100c100c0f0c100c0f0c100c100b100c100c0f0c100c0f0c100c100b100c100b100c100c0f0c100c100b2b0c0f0c100c0f0c2b0c2a0c2a0c2b0b100c2a0c100c000d05
```
