# Apache-Vhosts

A Python script, that automates the Apache Vhosts setup, for development purposes.

## Apache-Vhosts Quickstart

- Edit the script and add all the domains (names) that you wish to create on your local dev server.
- Run the script from your teminal with `sudo python apache_vhosts.py`.
- You can access each domain you provided at `http://eachDomainName.local/`. 

The scipt creates a `vhosts` directory under `/var/www/html/`.

Within the `/var/www/html/vhosts/` directory, a directory is created for each domain name, with a `public_html` directory, which is the webroot directory for the specific virtual host and a `logs` directory for the `error` and the `access` logs.

PS: Check the Python version you are using. For Python 3.5 you will have to uncomment the respective code within the script (check the comments). Python 2 is not supported. 