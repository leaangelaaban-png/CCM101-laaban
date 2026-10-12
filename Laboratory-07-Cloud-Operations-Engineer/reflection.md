# Laboratory 07 Reflection

Checking the host server's resources is important even when containers appear to be running properly. Containers depend on the host's available CPU, memory, and disk space. If these resources become limited, an application may slow down or stop responding. Checking system resources helps engineers identify possible problems before they affect the service.

The `docker logs` command helps engineers investigate application issues by showing recorded events and requests. In this activity, the logs showed three successful HTTP 200 requests and one HTTP 404 response for a missing page. If a user cannot access a page or log in, available logs can provide clues about failed requests and help engineers decide what to investigate next. Additional checks may be needed to identify the complete cause.

Logs and metrics provide different types of information. Logs record events, requests, and errors, while metrics show numerical measurements such as CPU usage, memory consumption, and network activity. Using both helps engineers understand what happened in an application and how it used system resources.

Companies can monitor thousands of containers using centralized monitoring tools. Prometheus can collect metrics, while Grafana can display those measurements in dashboards. These tools help teams observe performance trends and identify unusual resource usage across many containers without checking each one manually.

This activity helped me practice Linux commands and Docker monitoring tools. I learned how to check memory and disk capacity, deploy a web server, send HTTP requests, inspect access logs, and observe container metrics. I also learned that a running container does not automatically mean every request will succeed. Monitoring logs and metrics provides useful evidence when checking the health of a service.
