# Reflection — The Cloud Security Engineer

A host-based firewall protects an individual server by controlling the network traffic that can reach it. Even if the physical network perimeter is breached, the server can still reject incoming connections that are not explicitly permitted. This provides another layer of defense and helps reduce the risk of unauthorized access.

Managing open network ports is important because every exposed service creates another possible entry point for an attacker. If a server only needs SSH for administration and port 8080 for its web application, unnecessary ports should remain closed. Limiting access to required services follows the principle of least privilege and reduces the server's attack surface.

Leaving a database port such as 3306 for MySQL open to the public internet is dangerous because attackers could attempt unauthorized logins, exploit software vulnerabilities, or repeatedly guess credentials. A database often stores sensitive information, so it should be accessible only to trusted applications or administrators through controlled network rules. Strong authentication and other security controls are also necessary.

Completing this mission changed my perspective on how easily a server can become exposed when its security settings are not configured properly. Deploying an application is not enough; its network access must also be reviewed. I learned that checking firewall status and testing the application after changing rules are important steps in verifying security.

My GitHub portfolio now provides a record of eight cloud computing missions and the skills I have practiced. Each mission contributes to my understanding of cloud infrastructure, deployment, operations, and security. Organizing the work with Markdown documentation and screenshots also helps me review what I did and explain the evidence for each task. I understand that maintaining a portfolio requires accurate documentation and genuine evidence of completed work. This mission taught me to treat security as an ongoing responsibility rather than a one-time configuration.
