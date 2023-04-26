# ubuntu-ssh-enabled based on ubuntu 22.04


1. ```docker login -u isochau```

2. ```docker build -t isochau/ubuntu-ssh-enabled .```

```docker push isochau/ubuntu-ssh-enabled```

3. ```docker run -dit --name [Container Name] -p [PORT]:22 [IMAGE_NAME]```

```docker run -dit --name lab-ubuntu-ssh -p 22:22 isochau/ubuntu-ssh-enabled```

NOTE: THIS IMAGE IS TO BE USED FOR TEST AND LEARNIGN PURPOSES ONLY! NOT TO BE USED IN A PRODUCTION ENVIRONMENT!

SSH Enabled Ubuntu Image for Test and Dev purposes ONLY!

## Use:

Run the container:

```docker run -d isochau/ubuntu-ssh-enabled```

Identify the Internal IP

```docker inspect <container-id-name>```

SSH

```ssh <container-ip>```

**Username:** root

**Password:** password

Based on:
https://mtabishk999.medium.com/how-to-enable-ssh-within-a-docker-container-511260a70cce

