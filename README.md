# apt-cacher-ng
dockerized version of Apt-Cacher-ng

[![DockerHub Badge](https://dockeri.co/image/cutyno/apt-cacher-ng)](https://hub.docker.com/r/cutyno/apt-cacher-ng)

## Volume
- /var/cache/apt-cacher-ng : Cache volume
- /var/log/apt-cacher-ng : Vloume for log files
- /etc/apt-cacher-ng : Volume for config files

## Port
- 3142 : Port for proxy and for the apt-cacher-ng Interface

## Usage
you can run containers with: ```docker run -t -i --rm -e http_proxy http://dockerhost:3142/ debian bash```
Here, `dockerhost` is the IP address or FQDN of a host running the Docker daemon which acts as an APT proxy server.

Webinterface: http://dockerhost:dockerport/acng-report.html
