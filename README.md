# prex.io-vagrant
Vagrant configuration for prex.io machine with services, databases, &amp; sites.

Installation
---

* Recursively clone the Vagrant configuration
  ```sh
  git clone --recursive git@github.com:rex/prex.io-vagrant.git prex.io
  ```
* Initialize and update all submodules
  ```sh
  git submodule init
  git submodule update
  git submodule foreach git checkout master
  git submodule foreach git pull origin master
  ```
* Install the `librarian-chef` gem 
  ```sh
  gem install librarian-chef
  ```
* Install the Chef cookbooks
  ```sh
  librarian-chef install
  ```
* Start the server!
  ```sh
  vagrant up
  ```
