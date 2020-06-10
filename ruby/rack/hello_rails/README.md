# README

A simple Rails app that uses asset pipeline and uses the Rack (default rails) web server

## Get started:

1) `pack build` it using Paketo Node.js and Ruby buildpacks.  
```
pack build rails-rack-app --buildpack gcr.io/paketo-buildpacks/nodejs --buildpack gcr.io/paketo-community/ruby
```
2) `docker run` the app.
```
docker run -e PORT=9292 -p 9292:9292 -it rails-rack-app
```
