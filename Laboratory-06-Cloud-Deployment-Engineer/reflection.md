# Laboratory 06 Reflection

Using a docker-compose.yml file made the deployment easier because the settings for the different services were written in one configuration. Instead of preparing each container separately, Docker Compose could use the file to create the application and database services together. I learned that this approach can save time and make the deployment steps easier to repeat.

I also learned that YAML requires proper spacing and indentation. A Tab or incorrect number of spaces can change the structure of the configuration and may cause Docker Compose to reject the file. This made me more careful when creating configuration files because a small formatting mistake can prevent the services from starting.

Environment variables such as MYSQL_PASSWORD were used to provide the information needed for the database connection. The application needs the correct password, database name, username, and host so it can communicate with MariaDB. These values in the Compose file help connect the Nextcloud service to its database service.

Seeing Nextcloud become available through the browser made the activity more understandable for me. It was interesting to see that after running only a few Docker Compose commands, the setup page for a cloud storage application could already be accessed. It connected the terminal commands with an actual web-based application.

Since Mission 1, my understanding of Cloud Computing has expanded. I have learned that cloud computing involves different technologies working together, including containers, networking, databases, storage, Linux, and automation. This laboratory helped me understand how these concepts can be combined to deploy and manage a cloud application in a more organized way.
