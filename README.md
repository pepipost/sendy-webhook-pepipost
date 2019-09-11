[![N|Solid](https://camo.githubusercontent.com/229d5a801bc32845251f6df372b47f0ef61cd3e3/68747470733a2f2f70657069706f73742e636f6d2f77702d636f6e74656e742f75706c6f6164732f323031372f30372f505f4c4f474f2e706e67)](https://nodesource.com/products/nsolid)

[![Build Status](https://camo.githubusercontent.com/273b9129e7bb4dee23056cfea466054b6104b19a/68747470733a2f2f696d672e736869656c64732e696f2f7061636b61676973742f7068702d762f70657069706f73742f70657069706f73742d73646b2d7068702e7376673f7374796c653d666c61742d737175617265)](https://packagist.org/packages/pepipost/pepipost-sdk-php) [![Build Status](https://camo.githubusercontent.com/b52da95112b380731b1864a6f985718fce5822ba/68747470733a2f2f696d672e736869656c64732e696f2f747769747465722f666f6c6c6f772f706570695f706f73742e7376673f7374796c653d736f6369616c266c6162656c3d466f6c6c6f77)](https://twitter.com/pepi_post)

# Pepipost webhook extension for Sendy
This is an extension for the Sendy platform which allows the user to track mailing reports using webhooks through Pepipost emailing services.

We are trying to make our libraries community-driven and we need your help in building the right things the right way you. Your opinion is very much valued so please share comments, create [issues](https://github.com/pepipost/sendy-webhook-pepipost/issues) and [pull](https://github.com/pepipost/sendy-webhook-pepipost/pulls) requests.

# Table of Contents
  - [Installation](#Installation)
  - [Quick Start](#Quick-Start)
  - [About](#About)
  - [License](#License)
  - [Credits](#Credits)

# Installation
The installation of the Sendy webhooks requires the exact same steps on both Linux and Windows OS.

# Prerequisites
  - [PHP >=5.4.0](http://php.net/manual/en/install.php)
  - A [Sendy](https://sendy.co/) Installation on a preferred domain
  - A free account on Pepipost. If you don't have a one, click [here](https://app.pepipost.com/index.php/signup/registeruser?utm_campaign=GitHubSDK&utm_medium=GithubSDK&utm_source=GithubSDK) to signup and get 30,000 emails free every month.
  - Pepipost SMTP Integration with sendy (Please click [here](#) for sendy integraton tutorial)

# Quick Start
1. Check the PHP version using below command. Required PHP >=5.4.0.
    ```sh
    $ php -v
    ```
2. Go to your Sendy installation directory
    For example, if your Sendy installation is inside var/www/html inside your server directory then.
    ```sh
     $ cd /var/www/html
    ```
2. Clone this repository on your machine using below command:
    ```sh
     $ git clone https://github.com/pepipost/pepipost_webhook.git webhooks
    ```
3. Go to the config file directory
    ```sh
    $ cd /webhooks/includes/
    ```
4. Edit config.php
    ```sh
    $ vim config.php
    ```    
5. Check the following line of code at line 27
    ```sh
    include_once(dirname(FILE)."/../../includes/config.php");
    ```  
6. The directory mentioned in the above code should point to your sendy installation config file 
    ```sh    
    For example: {your-sendy-installation-path}/includes/config.php
    ```  

7. Go to your Pepipost account dashboard by logging into 
    app.pepipost.com

8. Go to your Pepipost webhooks panel at link 
    https://app.pepipost.com/app/settings/webhooks

9. Under the global API, tab paste your URL that should point to pepipost.php inside the webhooks folder and verify
    Your webhook URL should look something like this
    ```sh
    {your-sendy-installation-path}/webhooks/pepipost.php
    ```  
10. Click on verify if you want to check if the webhook integration is working properly

11. After verification click on "Add Webhook" button.

Please click [here](https://developers.pepipost.com/overview/what-is-webhooks/what-is-webhooks) for more information about Pepipost webhooks.

With these steps completed, you are now free to use Pepipost webhooks with Sendy to track the email status.

# About
Pepipost webhooks is a PHP extension for Sendy, that allows users with Sendy installation integrated with Pepiopst mailing service to be able to track email status through Sendy user panel.

# License
GNU General Public License v2.0

# Credits
This application uses an Open Source code. You can find the source code of their open-source projects along with license information below. Please refer the provided links for sources.

Credits to: BlaineMoore
Github link: https://github.com/BlaineMoore/sendy-webhooks
License: GNU General Public License v2.0

Credits to: itabrezshaikh 
Github link: https://github.com/BlaineMoore/sendy-webhooks/pull/10
License: GNU General Public License v2.0

