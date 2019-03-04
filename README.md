# Enviroment local - using Docker
## Run 
`docker-compose up` 
## Stop 
Key press `CTRL + C` to finish server and run:
```
docker-compose down
```

## Build base image
 `docker-compose up`
 `docker build -t githubpagebase:v1.0 .`

### Run image util commands
 From bash or powershell
 ```
 docker run --rm -it -p 4000:4000 -v ${PWD}:/app -w /app githubpagebase /bin/bash
 ```
 
 From windows command line
 ```
 docker run --rm -it -p 4000:4000 -v %cd%:/app -w /app githubpagebase /bin/bash
 ```

### Run jekyll serve:
```
bundle exec jekyll serve --host 0.0.0.0 -w --config "_config.yml,_config_dev.yml"
```

```
 > docker run --rm -it -p 4000:4000 -v %cd%:/app -w /app githubpagebase:v1.0 /bin/bash -c "'bundle install && bundle exec jekyll serve --host 0.0.0.0 -w --config '_config.yml,_config_dev.yml'""
```


# Start Web
`bundle exec jekyll serve -w ` execute serve with watching files.



# [Start Bootstrap - Landing Page](https://startbootstrap.com/template-overviews/landing-page/)


## Bugs and Issues


## About


## References

* https://startbootstrap.com

Start Bootstrap is an open source library of free Bootstrap templates and themes. All of the free templates and themes on Start Bootstrap are released under the MIT license, which means you can use them for any purpose, even for commercial projects.


## Copyright and License

Compostela Tech.
