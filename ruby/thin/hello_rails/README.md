# README

A simple Rails app that uses asset pipeline and uses the Thin web server

## Get started:

1) `pack build` it using Paketo Node.js and Ruby buildpacks.  
```
pack build rails-thin-app --buildpack gcr.io/paketo-buildpacks/nodejs --buildpack gcr.io/paketo-community/ruby
```
2) `docker run` the app.
```
docker run -e PORT=3000 -p 3000:3000 -it rails-thin-app
```
