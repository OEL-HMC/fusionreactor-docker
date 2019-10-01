# Lucee
There are many different version of [Lucee](https://hub.docker.com/u/lucee/) available on the Docker Hub.

# Installing FusionReactor
Installing FusionReactor into an existing Lucee image is simple. Add the fusionreactor.jar file and optionally the native library required for the Ultimate features. Then modify the LUCEE_JAVA_OPTS environment variable to append the javaagent and agentpath strings.

# Build image
e.g
docker build -t lucee-fusionreactor:latest

# Running Lucee
 docker run -d -v D:/WebServer/your_favorite_website/:/var/www/ -p 8080:8888 lucee-fusionreactor:latest

 # Lucee admin
 http://127.0.0.1:8080/lucee/admin/server.cfm
 http://127.0.0.1:8080/lucee/admin/web.cfm

 Both URLs will prompt to set your password

 # FusionReactor
 http://127.0.0.1:8088
 Where a serial number will be required to use FR