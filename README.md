# Nifi POC

## Getting started

Start the server
> ./bin/nifi.sh run

Ctrl+c to quit

Start the server in background
> ./bin/nifi.sh start

Stop the server
> ./bin/nifi.sh stop

### Access the web console

Open the link https://localhost:8443/nifi on browser

Default configuration generates a username and password. This can be found in [Nifi Installation Dir]/logs/nifi-app.log. Note that the password found in conf/login-identity-providers.xml will not work.

## Running Nifi on docker

Pull latest docker image
> docker pull apache/nifi:latest

Run docker image setting the nifi port as 8443
> docker run --name nifi -p 8443:8443 -e NIFI_WEB_HTTPS_PORT='8443' -d apache/nifi:latest

Examine the docker logs for username and password
> docker logs -f nifi

Signin to web console same as mentioned in the local setup

### References
- Overview https://nifi.apache.org/docs/nifi-docs/html/overview.html
- Refer User guide https://nifi.apache.org/docs/nifi-docs/html/user-guide.html
- Refer Developer guide https://nifi.apache.org/developer-guide.html


