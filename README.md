# TSBIN

Smart Garbage Bin


Installtion
```
sudo apt-add-repository ppa:mosquitto-dev/mosquitto-ppa
sudo apt-get update
sudo apt-get install mosquitto
sudo apt-get install mosquitto-clients
sudo apt clean
```

```
systemctl status mosquitto.service
systemctl stop mosquitto.service

mosquitto -v // for localhost
mosquitto -c ~/Documents/tsbin/test/test.conf -v // for ip4 address, check the test.conf
```

Pub : 
```
mosquitto_pub -h //ip4 address// -t //topic// -m "Message"
mosquitto_pub -h ${ip} -t test -m "Message"
```

sub 
```
mosquitto_sub -h //ip4 address //-t //topic//
mosquitto_sub -h ${ip}-t test
```
