# NSA-20029677
Network Systems and Administration 


Kindly find the yaml file named as docker_deploy.yml

Please find the below pseudocode 

Deploy Docker container with React app using Apache:

1. Start Docker service:
   - Check if Docker service is running.
   - If not running, start Docker service.

2. Ensure /tmp/network directory exists:
   - Check if the /tmp/network directory exists.
   - If not, create the directory.

3. Create Docker network:
   - Define a Docker network named "apache_network" with IP subnet 172.168.10.0/30.

4. Create Docker container with Apache:
   - Define a Docker container named "react_container".
   - Use the httpd:latest image.
   - Map port 80 on the container to port 80 on the host.
   - Mount the /tmp/network directory on the host to /usr/local/apache2/htdocs in the container.
   - Attach the container to the "apache_network" network.

5. Copy React app build files to the host:
   - Copy files from /home/muthu/Retro/ to /tmp/network/ directory on the host.

