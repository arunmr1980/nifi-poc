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

### References
- Overview https://nifi.apache.org/docs/nifi-docs/html/overview.html
- Refer User guide https://nifi.apache.org/docs/nifi-docs/html/user-guide.html
- Refer Developer guide https://nifi.apache.org/developer-guide.html
