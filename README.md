# python-docker-app
python-docker-app

How to run a docker container with Newrelic key and enable monitoring

First way of execution as below and other format followed:

docker run -p 5000:5000 -e NEW_RELIC_LICENSE_KEY=xxxxx -e NEW_RELIC_APP_NAME=python-app manee2k6/py-newrelic

other format:

# Pre-requisite:
  Build a images with newrelic.ini specifying license key and app name in it and run the docker image.

docker run -p 5000:5000 -e NEW_RELIC_CONFIG_FILE=newrelic.ini pyapp-amrita
