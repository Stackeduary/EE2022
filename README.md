# Procedure to install Elasticsearch and Kibana

1. Ensure Docker and Docker Compose are installed and running.

2. On the command line, run `echo 'vm.max_map_count=262144' >> /etc/sysctl.conf` to increase the virtual memory available. 
    1. Run `sysctl -p` to apply the changes.
    2. Verify that the changes were applied by running `sysctl vm.max_map_count`.

3. On the command line, CD to the directory where you want to install Elasticsearch and Kibana.

4. `git clone git@github.com:Stackeduary/EE2022.git` to clone the repository.

5. `cd EE2022`

6. `docker-compose up -d` to start the containers.

7. `docker-compose ps` to check the status of the containers.

8. Open the browser and navigate to http://localhost:5601.

9. Verify that the Kibana dashboard is working.