Role Name
=========

Simple role that installs docker-compose service as a systemd service. 

Requirements
------------

System with locally installed docker-compose, docker, docker-python, and systemd. 

Role Variables
--------------

    DOCKER_COMPOSE_WORKDIR: "/compose"
    DOCKER_COMPOSE_APP_NAME: "docker-compose-service"
    
    # Local file containing docker compose service description
    DOCKER_COMPOSE_FILE: null
    
    # A mapping containing envirnment variables to be passed to docker-compose.
    # These variables will be stored to {{DOCKER_COMPOSE_WORKDIR }}/.env load this file in your
    # compose file. 
    DOCKER_COMPOSE_SERVICE_VARS: {}
    
    # If you use private registry fill service, username and password.
    DOCKER_LOGIN_SERVICE: null
    DOCKER_LOGIN_USERNAME: null
    DOCKER_LOGIN_PASSWORD: null



Dependencies
------------

None

License
-------

MIT
