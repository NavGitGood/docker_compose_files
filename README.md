# docker_compose_files
docker compose files for different ready to use services

1. postgres (port:5432) with pgadmin service (port:8080)
    - on pgadmin connect screen, use pgadmin credentials for login
    - to connect to postgresql database
        - name -> container-name
        - host name/address -> service name
        -


# how to use
1. create a .env file in the folder of service you want to run (select from env template directory) and enter the values
2. to run `docker compose -f {file_name} up -d`
3. to stop `docker compose -f {file_name} down`

# how to access on local network
1. get the ip address of the machine where docket container is running by executing ip -br addr show, and get the ipv4 for interface starting with either enp (ethernet) or wlp (wireless)
2. use that address along with the mapped port on the client machine to connect
