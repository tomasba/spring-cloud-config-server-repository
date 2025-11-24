configuration defined in the service applicication.yml takes precedence and may overwrite the config-server properties.
so it makes sence removing the properties from appropriate module application.yml

The properties/yml files naming:
- config-client.yml - it is like application.yml base properties file
- config-client-twitter_to_kafka.yml - here we have a profile usage named 'twitter_to_kafka'

The config-server is referring to the repository making it available to point from other modules with bootstrap.yml 
with spring.cloud.config.name and active profiles