---
tags:
- Development
- AngularJS
- Vagrant
---

# 🖼 The Framework

![Panel building](../../_assets/panel-building-construction.jpg)

## TL;DR

1. Cross-team code sharing is not worth finger pointing situations.
2. If you really, really feel that cross team code sharing make sense for your company, make sure that team behind the code, have more than enough time and resources to develop and provide support for other teams. In general just don't, it's huge investment which is mostly not worth of trouble.
3. Make sure that teams are motivated to maintain own dev stack and therefore onboarding and third party debuging is simply single command away. This makes team better understand deployment process and save them and others a lot of time on the way.

## Ambicious project

I was hired to be frontend developer to very ambitious project called simply the Framework, basically it was meant to be baseline for all Homecredit applications as backend based on Java and frontend based on AngularJS. Original assignment was to use 
Metawidget project to generate all the boring forms and views. I have decided that we have to go beyond and created render engine which I in lack naming enlightenment named simply the View. All our users ( developers ) has to do was create static json file where they defined pages and components they want on these pages and View generated whole app UI for them. Only limitation was their imagination and list of our AngularJS components. It wasn't perfect, but it worked and from my perspective it was huge success. When I saw one team which created workflow app, using our framework simply by dynamically generating view json file I was amazed 🙌.

## Success

We had first working prototype in few months and we were adding new components, fixing old ones and in spare time try to keep documentation up to date and most importantly trying to help teams with onboarding and issues. As there was just eight of us ( 4 backend and 4 frontend ) it was really hard to keep up with all teams. We were stuck between teams requesting new feature requests and teams screaming at us with bug reports. Bug reproduction was specially hard as it was not easy to just fire single command to start team application and reproduce their bug report steps. Their java applications required specific setup, so I have created Vagrant setup to be able to reproduce problems. It kind of worked, till they changed something in their setup and I had to update Vagrantfile accordingly. They simply didn't care about app execution outside of their dev env - this is really important experience I leveraged later. 

## Finger pointing downfall

As teams were pushed to quickly deliver or point a finger, they obviously start point fingers at us. This was the beginning of the end of the Framework project. More fingers more delays in deliveries, destabilised our ground. No matter how hard we tried to deliver features and no matter how hard we tried to resolve teams issues as soon as possible, there was simply too many fingers pointing at us. After some point it was decided that shared code is no longer viable and project was terminated. It was hard to see such project to fail, after so many effort put in to it 
