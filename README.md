Scripts I use to quickly deploy a Ruby on Rails app on Ubuntu 16.04.

Deploying a Rails app is normally a long process, but with these scripts, it takes me about ten minutes.

Run my-rails-new on your development environment. Use it like 'rails new' but with additional arguments. It will set up a new rails app with Capistrano, Bootstrap, and a hello, world page.

my-rails-new <app-name> <git-repository> <server-ip-or-domain> <user-name> <secret-key-env-var-name> <database-password-env-var-name>

Run rails-server-setup on a fresh install of Ubuntu 16.04 to install all the requirements: Ruby, Rails, PostgreSQL, Nginx, and more.

rails-server-setup <username>

Run rails-app-setup on the Ubuntu 16.04 server to prepare it for the deployment.

rails-app-setup <app-name> <secret-key> <secret-key-env> <database-password-env> <setup-host?(y/n)> <setup-ssl?(y/n)> <ip-or-domain> <username>