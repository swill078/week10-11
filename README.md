![MHN_Admin_Application](https://user-images.githubusercontent.com/78439538/116151062-262ffa00-a6b2-11eb-9f28-3751967fc29e.gif)
![snsors](https://user-images.githubusercontent.com/78439538/116151068-28925400-a6b2-11eb-9ee1-d9a35f2965ef.png)
# week10-11


Milestone 0: To the Cloud!

Milestone 1: Create MHN Admin VM

Milestone 2: Install the MHN Admin Application

Milestone 3: Create a MHN Honeypot VM

Milestone 4: Install the Honeypot Application

Milestone 5: Attack!

Configuration of mhn and vm instances actually took a lot of time but overall all the issues had been resolved.

ERROR 1: Killed python initdatabase.py. Once run $ sudo supervisorctl status, only geoloc, honeymap, hpfeeds-broker and mnemosyne are running.

ERROR 2: mhn-celery-worker do not running (solution: undate python version to 3.2.1 or higher in mhn-admin VM)

ERROR 3: When connect honeypots to mhn-admin always return a failure message: connection time out. (solution: check/rebuild mhn-admin and mhn-honeypot firewall. Also try to run [$ sudo apt-get update] and [$ sudo apt-get install software-properties-common -y] in mhn-honeypot ssh)


103.213.208.26 (366 attacks)

105.101.105.47 (196 attacks)

111.230.113.70 (182 attacks)

185.176.27.186 (130 attacks)

187.38.221.54 (126 attacks)

TOP 5 Attacked ports)

23 (802 times)

5060 (748 times)

445 (635 times)

8088 (488 times)

1433 (264 times)
