# tidbyt-manager
This is a very basic flask app for managing externally run applets for your tidbyt.  

default login in admin / password

docker needs port 8000 and 5100-5120 port range opened up (use --network=host to make it easy ((doesn't work on mac docker though))

set DOMAIN value in .env file if not running locally

https://github.com/tavdog/tidbyt-manager/assets/8324295/e83a8795-3cb9-40cb-b854-90d07df8aebd

## Running
1. `docker build . -t tidbyt:latest`
1. `docker run --name tidbyt -e DOMAIN=localhost -p 8000:8000 -p 5100-5120:5100-5120 -d tidbyt:latest`
1. Go to `http://localhost:8000/auth/register` and create a user account
2. Log in with that account


