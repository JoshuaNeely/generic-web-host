# generic-web-host

nginx and docker-compose configuration magic used to:  
* serve a website out of `./static-html` at port 80
* serve files out of `./exposed-filesystem` at port 8000
* serve arbitrary api requests with a flask container at port 8080

Tightly coupled to one particular project, but generic enough to live on its own.  
Volume mounts allow separating this website deployment from the content being deployed.  
Dynamic detection of services and files via flask api.  
