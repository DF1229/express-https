# express-https

## What is this?
This repository aims to provide a simple placeholder to test the validity and functionality of your HTTPS settings.

This project was made and tested on a system running Linux, specifically Ubuntu 18.04 LTS. 
Other operating systems should work fine, but feel free to open an issue if you find any bugs.

## Download & use
### 1. Download using the Git CLI, or your prefered method.
`git clone https://github.com/DF1229/express-https`

### 2. Install the dependencies using npm.
`npm install`

### 3. Upload your SSL key and certificate.
Locate and update the `sslcert/key.pem` and `sslcert/cert.pem` files accordingly.
*Need help generating an SSL certificate? See https://certbot.eff.org*

### 4. Run the index.js file
`node index.js`

### 5. Verify the server is running
Console output should look like this:

```
HTTP:80 LISTENING
HTTPS:443 LISTENING
```

Anything else means it's not working, refer to the error displayed on the console for more info.

## Common issues
### Connection timed out
Make sure you have opened port 443 (HTTPS) in your firewall and/or router.

For more on how to do this on Linux, see [this tutorial by DigitalOcean](https://www.digitalocean.com/community/tutorials/how-to-setup-a-firewall-with-ufw-on-an-ubuntu-and-debian-cloud-server) on the topic.
