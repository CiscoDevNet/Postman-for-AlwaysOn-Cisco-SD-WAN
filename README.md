# Postman for Cisco SD-WAN

This public repo contains a [POSTMAN](https://getpostman.com) environment and collection that can be used to interact with the `Cisco SD-WAN vManage REST API`. The environment is pre-configured to access the [Cisco DevNet Always On Sandbox for SD-WAN 19.2](https://devnetsandbox.cisco.com/RM/Diagram/Index/fa7f7ef9-e224-4ee7-a3fe-0f25506e9db9?diagramType=Topology) fabric. You can edit the variables in the environment to point to your own vManage instance. The collection contains REST API calls to authenticate, get a list of devices that are part of the SD-WAN fabric, and get device status, counters, and interface statistics for all the interfaces in the fabric. Feel free to modify them as you see fit and to add more calls to the collection.

![Sandbox Image](./images/sdwan_sandbox.png)

# Requirements

The Postman collection and environment will need:
* Postman 6.4.4+
* Cisco SD-WAN vManage 19.2.2

# Setup

If you don't have Postman already installed, you can download it from [here](https://getpostman.com). Once you install it, you can follow the steps below to import the collection and environment:

![Postman Image](./images/postman.png)

1. Click on `Import`, browse to the location where you cloned this repo and add the two files:
    1. `Cisco-AlwaysOn-SD-WAN-Env.postman_environment`
    2. `Cisco-AlwaysOn-SD-WAN.postman_collection.json`
2. Make sure you select the `Cisco-AlwaysOn-SD-WAN-Environment` environment
3. Expand the collection and start making REST API calls.

## Note: In case your instance of vManage has a self signed certificate, make sure you disable `SSL certificate verification` in Postman's settings.

To disable SSL certificate verification go to Settings, click on switcher as in the screenshot below

![SSL certificate verification](./images/postman_ssl_verification.png)


## About me

Network Automation Developer Advocate for Cisco DevNet.
I'm like Hugh Hefner... minus the mansion, the exotic cars, the girls, the magazine and the money. So basically, I have a robe.

Find me here: [LinkedIn](https://www.linkedin.com/in/stuarteclark/) / [Twitter](https://twitter.com/bigevilbeard)
