# Folding@Home on Raspberry Pi

***Folidng@Home*** allows you to contribute compute in order to assist and contribute to scientific research like disease research and molecular biology.

## Prerequisites
- Raspberry Pi (preferably Raspberry Pi 5 for better performance)
- Raspberry Pi OS
- An internet connection
- Cooling solution

# Steps
1. Setup your environment
   ```sudo apt-get update```
   
   ```sudo apt-get upgrade -y```
   
   ```sudo apt-get install -y libopenmpi-dev openmpi-bin```
   
   ```wget https://download.foldingathome.org/releases/public/release/fahclient/debian-stable-arm64/v7.6/fahclient_7.6.21_arm64.deb```
   
   ```sudo dpkg -i --force-depends fahclient_7.6.21_arm64.deb```
3. Configure ***Folding@Home***
   - Username
   - Team number
   - Passkey
   - Enable folding power auto-adjustment
   - Allow remote access
4. Start the ***Folding@Home service***
   ```sudo /etc/init.d/FAHClient start```
5. Monitor the service
   ```sudo apt-get install fahcontrol```
   
   ```fahcontrol```

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

### Author
[Tengis Zuchi](https://github.com/tengiszuchi)


