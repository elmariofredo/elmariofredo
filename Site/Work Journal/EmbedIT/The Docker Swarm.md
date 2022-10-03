# 🚂 The Docker Swarm

![]()

During the Framework times I started experimenting with docker. Mainly as replacement for Vagrant which was quite heavy for this purpose. I have pitched docker idea to one coworker which had task to prepare scripted installation for our application suite. It was too huge task and obviously failed, but docker idea resonated to upper management. When our team no longer had any purpose, management came out with idea to containerise all applications. It was perfect task for me and just in time to pour fresh dose of enthusiasm to start something new.

I jumped right into training teams about docker and containers, this gave teams safe space where they can learn new technology. This also forced me look more deeply into how docker works. Parallel to education we started building container platform, based on Docker Swarm running on RHEL linux OS. Quickly we started bumping into issues with docker on old linux kernel and most importantly we started running into missing Docker Swarm features, which our enterprise apps desperately needed. We tried add #Ansible to keep up with teams request and quickly realized that this wasn't the right solution. Yes docker compose file was "simple" compared to Kubernetes yaml hell, but our ansible monster was way worse. 

## 🗝 Key notes

1. When bringing new technolog 

We started from scartch and this time we jumped on Kubernetes bandwagon
