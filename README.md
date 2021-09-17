# _Infrastructure-docker-compose-nextcloud_
Creating an infrastructure to host NextCloud.  All the components that compose it are managed with Docker-Compose, the effort to configure and manage the application is minimal.
## Infrastructure consists of the following components:
- **PostgreSQL**
  *is a free and open-source relational database management system (RDBMS) emphasizing extensibility and SQL compliance.*
- **SWAG - Secure Web Application Gateway**
  *(formerly known as letsencrypt, no relation to Let's Encrypt™) sets up an Nginx webserver and reverse proxy with php support and a built-in certbot client that automates free SSL server certificate generation and renewal processes (Let's Encrypt and ZeroSSL). It also contains fail2ban for intrusion prevention.*
- **NextCloud**
  *Nextcloud gives you access to all your files wherever you are. Where are your photos and documents? With Nextcloud you pick a server of your choice, at home, in a data center or at a provider. And that is where your files will be. Nextcloud runs on that server, protecting your data and giving you access from your desktop or mobile devices. Through Nextcloud you also access, sync and share your existing data on that FTP drive at the office, a Dropbox or a NAS you have at home.*

### Docker images:
- [***PostgreSQL***](https://hub.docker.com/_/postgres): postgres:9.6.23-stretch
- [***NextCloud***](https://hub.docker.com/r/linuxserver/nextcloud): linuxserver/nextcloud:php8-version-22.1.1
- [***Swag***](https://docs.docker.com/compose/): linuxserver/swag:version-1.19.0

## Deployment method:
[***Docker***](https://docs.docker.com/compose/) is a set of platform as a service (PaaS) products that use OS-level virtualization to deliver software in packages called containers. Containers are isolated from one another and bundle their own software, libraries and configuration files; they can communicate with each other through well-defined channels.Because all of the containers share the services of a single operating system kernel, they use fewer resources than virtual machines.

[***Docker-Compose***](https://hub.docker.com/r/linuxserver/swag) is a tool for defining and running multi-container Docker applications. With Compose, you use a YAML file to configure your application’s services. Then, with a single command, you create and start all the services from your configuration.*

---
