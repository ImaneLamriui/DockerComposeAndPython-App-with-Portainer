## Requirements: Flask framework
__Flask is a framework for Python__, so you need to have Python installed on your system. Flask is compatible with Python 3 and higher versions.

__Installation of Flask__: You need to install Flask in your development environment. You can do this using pip, the Python package manager. You can install Flask by running the following command in the terminal or command prompt:

###### pip install Flask

### Using Docker Compose with __Portainer__ allows you to manage your multi-container Docker applications more conveniently, as you can define and manage all your containers in a single configuration file.
__Portainer__ simplifies the management and deployment of Docker containers, making it particularly useful for teams looking to efficiently utilize Docker without dealing with the complexity of the command line.

__https://docs.portainer.io/#documentation__

__Portainer itself is deployed__ as a Docker container, which means you can run it within your existing Docker environment to manage your other containers more conveniently.

To download and start Portainer:

You can download and start Portainer as a Docker container using the following command:
###### docker run -d -p 9000:9000 --name=portainer --restart=always -v /var/run/docker.sock:/var/run/docker.sock portainer/portainer-ce
This command will download the Portainer image from __DockerHub__ and start it as a __container named "portainer"__. 

The   __-v /var/run/docker.sock:/var/run/docker__. sock option allows Portainer to access the Docker socket to manage the containers.

__Access Portainer__: Once Portainer is up and __running__, you can access its web interface from your web browser by visiting __http://localhost:9000__ ,  Or with __https__ protocol on port 9443:  __https://localhost:9443/__ (__docker run -d -p 9443:9443 --name=portainer --restart=always -v /var/run/docker.sock:/var/run/docker.sock portainer/portainer-ce__) or (__http://<your_ip_address>:9000 or http://<your_ip_address>:9443__) if you are running Docker on a __remote machine__. 

Next, follow the instructions to set up Portainer, including __creating an admin user and connecting to Docker__.

Once you have configured Portainer, you can use its web interface to manage your Docker containers more easily and intuitively, including __creating, modifying, monitoring, and deleting containers, among other functionalities__.

__https://docs.portainer.io/start/agent__

__https://portal.portainer.io/knowledge/licensing__
