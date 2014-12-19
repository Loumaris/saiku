loumaris-saiku
==================

Base docker image to run a saiku server


Saiku version
-------------

Currently it is version 3.0.7

Usage
-----

To create the image `loumaris/saiku`, execute the following command on the loumaris-saiku folder:

        docker build -t loumaris/saiku

or just pull it from the dockerhub (recommended):

        docker pull loumaris/saiku

To run the image and bind to port 8080 (default):

        docker run -d -p 8080:8080 --name saiku loumaris/saiku

The first time that you run your container, a new user `admin` with all privileges 
will be created in saku with the password `admin`. 

To add your licence go to http://your-host:8080/upload.html and drop your licence file.

To use your data source (e.g. MySQL) you can link the saiku container with your source as you know. 
You can connect the source from the backend settings after it.

Done!