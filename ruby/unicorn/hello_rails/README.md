# README

A simple Rails app that uses asset pipeline and uses the Unicorn web server.  

## Get started:

1) `pack build` it using Paketo Node.js and Ruby buildpacks.  
```
pack build rails-unicorn-app --buildpack gcr.io/paketo-buildpacks/nodejs --buildpack gcr.io/paketo-community/ruby
```
2) `docker run` the app.
```
docker run -e PORT=8080 -p 8080:8080 -it rails-puma-app
```
