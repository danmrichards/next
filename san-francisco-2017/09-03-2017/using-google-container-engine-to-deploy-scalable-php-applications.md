# Using Google Container Engine to Deploy Scalable and Secure PHP Applications

## Advantages of Compute Engine for PHP
* Easy to spin up apps like WordPress (via cloud launcher)
* Easy to spin up LAMP stack (via cloud launcher)
* Low barrier of entry (it's just VMs people!)
* Autoscaling instance groups
* Easy SSL firewall

## Advantages of using the PHP base image
* Automatic composer installation
* PHP 5.6, 7.0 and 7.1
* Logging integration with Google Cloud Logging
* Error handling integration with Google Stack Driver
* NGINX
* Easy **php.ini** configuration
* Easy web server configuration
* Pre-installed shared extension which can be activated in **php.ini**

## Security Advantages
* PHP and extensions are kept up to date
* Security patches
* Suhosin security logging
* No **.htaccess**
* Appropriate file permissions

## App Engine Advantages
* Versioning with containers and URLs
* Autoscaling
* SSL by default on *.appspot.com
