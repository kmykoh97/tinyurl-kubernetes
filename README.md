# Scalable 'Tiny url' app example
This project demonstrates deployment and scaling of the famous tiny url app using kubernetes.
Project can be run and tested on your laptop with docker-compose and  be deployed on kubernetes without code modification

Tiny url app is often used as an example to demonstrate various aspects of software scaling due its simplicity. Essentially it has following functions:
- Given a long url, convert it to a short url
- Given short url, return the original url

Thats it, however please do not underestimate the challenge here, you can still run into nearly all of the bottlenecks that you would see in a more 'complex' application :)

Our 'Tiny url' application will be made out of 3 services:
- Django rest server
- Redis cache
- Postgres database

Here the Django rest server will orchestrate redis and postgres to perform its functions
