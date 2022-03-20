# Tips to connect to virtual machine via VS code

## Scenario
- Host Ubuntu Desktop XX.YY
- Guest Ubuntu Server XX.YY (Running on Virtual box 5) Problem
- SSH connection refused

## Solution on putty
1. Shut your guest Ubuntu down
2. On Virtualbox go to Setting>network>Adapter1>Advanced>Portforwarding
3. Name=SSH Hostport=2022 (or any port but 22) Guestport(22)
4. Reboot your guest or virtual machine
5. On you host open a Putty or whatever you use for SSH
6. ssh user@127.0.0.1 -p2022 (or any port you mentioned as hostport)

## Solution on VS code
1. Install Remote Explorer SSH plugin
2. Click on the add config on top of side window
3. Enter ssh user@127.0.0.1 -p2022 (user is the VM login name)
4. Chosse the folder where config need to be stored
5. Choose the type of OS you have in VM
6. Open config file and make sure **hostname** is 127.0.0.1 and **port** is 2022
7. **User** should your VM machine login name

Have fun you are in
