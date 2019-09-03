# Details
> Galois is an auto code completer for code editors (or any text editor) based on OpenAI GPT-2. 

Docker Compose file for the [Galois Web Interface](https://usegalois.com/).
This compose file consist of four Docker images:
- Here [Galois](https://github.com/iedmrc/galois-autocompleter) used as autocompleter. It works on nvidia runtime by default and returns *code completion predictions* for the code given. If you want to run *Galois* on CPU, please follow the link [here](https://github.com/iedmrc/galois-autocompleter#with-docker).
- The [Web](https://github.com/iedmrc/galois-web) image serves an *Vue* based online code editor for [Galois](https://usegalois.com).
- [Nginx Proxy](https://github.com/jwilder/nginx-proxy) is a popular Nginx reverse proxy image by [jwilder](https://github.com/jwilder).
- [Nginx letsencrypt](https://github.com/JrCs/docker-letsencrypt-nginx-proxy-companion) is a lightweight companion container image for nginx-proxy.

Check the [Galois](https://usegalois.com/) for more details.