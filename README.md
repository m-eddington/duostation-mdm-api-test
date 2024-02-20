# duostation-mdm-api-test
Quick and dirty bash script for testing the duostation mdm api by sending a message to a managed device.

Requires curl.

Usage
./api-test.sh DeviceSerialNumber "message to send"

Use a list of serial numbers with a while loop for sending the message to more than one device
cat snlist.txt | while read line; do ./duostation.sh "$line" "message to send"; done 

The full API documentation can be found at https://duostation.com/news (check for the latest post about the API)
