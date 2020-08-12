# README

A simple Rails app that uses asset pipeline and uses the Passenger web server.  

## Get started:

1) `pack build` it using Paketo Node.js and Ruby buildpacks.  
```
pack build rails-passenger-app --buildpack gcr.io/paketo-buildpacks/nodejs --buildpack gcr.io/paketo-community/ruby
```
2) `docker run` the app.
```
docker run -e PORT=3000 -e RAILS_ENV=development -p 3000:3000 rails-passenger-app
```
