# README

This README would normally document whatever steps are necessary to get the
application up and running.

Things you may want to cover:

* Ruby version

* System dependencies

* Configuration
  build based on tutorial from https://docs.docker.com/compose/rails/#build-the-project

* Database creation
  $ docker-compose run web rake db:create

* Database initialization
  $ docker-compose run web rake db:migrate
  $ docker-compose run web rake db:seed

* How to run the test suite

* Services (job queues, cache servers, search engines, etc.)
  start the server
  $ docker-compose up
  stop the server
  docker-compose down
  docker-compose run web rails g scaffold User name
  docker-compose run web rails c

  If you make changes to the Gemfile or the Compose file to try out some different configurations, you will need to rebuild. Some changes will require only
  $ docker-compose up --build

* Deployment instructions

* Problems
  You might have to remove the tmp/pids/server.pid file

* Build a docker images
  docker build -t composeandrails .

* Tag and push image to docker hub
  docker tag composeandrails synthmax/compose-and-rails:part1
  docker push synthmax/compose-and-rails:part1

* ...
