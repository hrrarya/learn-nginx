## Learn Nginx

Nginx is a simple web server. it is used to server content in the server. but it is not just a server, it also covers reverse proxy, caching, load balencing, static file serving etc. 


now I will discuss about its configuration. 

Nginx configurations are a set of rules for nginx. in configuration file, we can define how nginx will act, what it will do. 

I am using docker for nginx installation. i have installed nginx:1.28.3-alpine image from docker hub. 

linux configurations are saved in the /etc/{SERVICE_NAME}/ folder. so in our case the nginx configurations are in the `/etc/nginx/` folder. inside this folder, we can see several files. but i will talk about nginx.conf file now.


this is the main configuration file for nginx. in this file, we can define everything we want to do done using nginx. 

let me talk about its basic structure a little bit.

Main
    - Events Block
        - in this block, we can define how many worker connection will be used
    - Stream Block
        - in this block, we work with advanced ports like tcp/udp
    - HTTP Block
        - Server Block
            - in this block, we define configurations for serving contents, caching, load balencing etc. 
        - Upstream Block
            - if we want to use nginx as reverse proxy, then we need this upstream block. 
        


