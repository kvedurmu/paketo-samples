# README

A simple Rails app that uses asset pipeline and uses the Puma web server. Generated using `rails new <PROJECT>`.  

## Get started:

1) `pack build` it using Paketo Node.js and Ruby buildpacks.  
```
pack build rails-puma-app --buildpack gcr.io/paketo-buildpacks/nodejs --buildpack gcr.io/paketo-community/ruby
```
2) `docker run` the app. Note that Puma defaults to port `9292`.
```
docker run -e PORT=9292 -p 9292:9292 -it rails-puma-app
```
