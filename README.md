# vagrant-shopify-app
(c) Andre Lohmann (and others) 2019

## Maintainer Contact
 * Andre Lohmann
   <lohmann.andre (at) gmail (dot) com>

## content

Vagrant template, to run the shopify tutorial at https://developers.shopify.com/tutorials/build-a-shopify-app-with-node-and-react/embed-your-app-in-shopify

Instead of ngrok, this vagrant machine uses localtunnel.me to create a secure tunnel from the public internet to your local machine. The subdomain, you want to use is set in ansible_vagrant/custom_vars.yml as well as the shopify shop url and your app api key and secret.

## Usage

### Configuration

  * Copy the config.yml.example to config.yml and alternate as you need it.
  * Copy the ansible_vagrant/custom_vars.yml.example to ansible_vagrant/custom_vars.yml and alternate as you need it.

### Run

```
vagrant up
```

Change the files in /application and watch the changes live using your configs domain or your localtunnel.me subdomain

```
http://YOUR.CONFIGS.DOMAIN:3000
```
