## This repository is used to configure the entire link shortener project. 
It uses docker-compose to setup and run the project.

 Before starting the project, download [shorten_links_frontend](https://github.com/mikolajlinkshortener/shorten_links_frontend) and [link_shortener_backend](https://github.com/mikolajlinkshortener/link_shortener_backend).

Your project structure should look like this:

    Projcet  
    ├── .env.dev 
    ├── docket-compose.yml  
    ├── shorten_links_frontend      # downloaded repository  
    ├── link_shortener_backend      # downloaded repository  
    ...  

In .env.dev are variable only for development. SHORT_LINK_LENGTH configure how long is generated part of short link. 

Run in root directory comands :
```
docker-compose build
docker-compose up
```

TO_DO run migrations in Dockerfile  
Go to django container and run migrations

*Pro tip:  
Open both backend and frontend in diffrent VSC Windows, do not use this repo for development.

