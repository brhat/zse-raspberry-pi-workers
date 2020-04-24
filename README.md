# zse-raspberry-pi-workers
dockerized buildbot-workers for various versions of the raspberry-pi

Prerequisites:
- you have to have docker and docker-compose installed. 
- add your unprivileged user to the docker group

Setup:
1: clone / copy this repository to a raspberry-pi.
1.1: (Optional) Create a branch for your configuration including secrets (git checkout -b secrets)
2: modify URL and port of the buildmaster in buildmaster.env.
3: cd into the folder fitting your model (run uname -m if you are unsure)
3.1: modify the passphrase and worker name in the .env file
3.2: make sure that the buildmaster is configured with the same values
5: run docker-compose up -d
