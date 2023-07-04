# Grafana-integration-with-MYSQL-DB

Devops Project: Grafana Integration with MySQL DB on AWS

Grafana Is a dashboard tool we can use it for system health checks, system matrices, cpu utilisation, number of apps running, graphs and much more , For the metrics to come on Grafana we need data and establish a connection between database and Grafana, here in the my SQL db we will create a db, table, insert the data and make sure it communicates

We will be having two Docker containers with volumes, one for Grafana and other for MySQL db .Pull the Grafana Docker image from the official repository and create a container. Mount a volume to persist Grafana's data ,Similarly, pull the MySQL Docker image and create a container. Mount a volume to persist MySQL's data. Configure the necessary environment variables to set up the root password and other MySQL settings.

Then we will add a data source in Grafana as my SQL , Access the Grafana web interface using the EC2 instance's public IP address and the appropriate port (default is 3000). Log in to Grafana and navigate to the data sources section. Add a new data source, selecting MySQL as the type. Provide the necessary connection details, including the host, port, database, username, and password.

in Grafana one of the best things is we can add many data sources, data sources are nothing but integration of tools , then we will be writing queries to extract the data from db to dashboard, By this You can view the real-time metrics and visualizations provided by Grafana, sourced from your MySQL database.

Below are the steps involved in the process:

a) create an ece instance, go to the security group and allow all traffic

b) install Docker, enable docker then create a container for Grafana

c) install MySQL and create a container for it

d)use the 'exec' command to go inside the container

e) create username and password for logging in database

f) create a new database, use this db and create a table inside it then insert the data

g)add data source in Grafana as MySQL

h)add a dashboard with a panel

i)write the query to extract the data from mysql and display it on the dashboard
