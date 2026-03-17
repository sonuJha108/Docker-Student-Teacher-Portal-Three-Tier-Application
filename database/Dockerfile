# Use the official MySQL 8.4 image as the base image
FROM mysql:8.4

# Set the root password for MySQL
ENV MYSQL_ROOT_PASSWORD=mysql123

# Create a default database named 'school' when the container starts
ENV MYSQL_DATABASE=school

# Expose port 3306 so MySQL can be accessed from outside the container
EXPOSE 3306

# Create a volume to persist MySQL data even if the container is removed
VOLUME [ "/var/lib/mysql" ]

# Run the MySQL server when the container starts
CMD [ "mysqld" ]