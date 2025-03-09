# Securing-an-Apache-Web-Server

## Objective

Let's fortify our Apache web server on Ubuntu with strong security measures. This will protect sensitive data, keep our service running smoothly without interruptions, and maintain the integrity of our system against potential threats. By proactively boosting our server's security, we're committed to providing a safer and more reliable environment for our users and stakeholders.

### Skills Learned

- **System Administration:** Managed Ubuntu server efficiently.
- **Web Server Configuration:** Installed and configured Apache.
- **Firewall Management:** Secured server with UFW rules.
- **SSL Implementation:** Used Let's Encrypt for HTTPS.
- **Virtual Hosts:** Configured multiple websites on a single server.
- **Security Best Practices:** Applied measures like ModSecurity and disabling directory listings.
- **Monitoring:** Regularly updated and monitored server health.
- **Troubleshooting:** Resolved security and performance issues.

### Tools Use

- **Apache2:** For web server setup and configuration.
- **UFW (Uncomplicated Firewall):** To manage firewall rules and enhance security.
- **Certbot:** To obtain and install SSL certificates from Let's Encrypt.
- **ModSecurity:** To provide web application firewall protection.
- **Fail2Ban:** For monitoring and protecting against brute-force attacks.

## Steps

Step 1 : Installing apache2 

![installation](https://github.com/user-attachments/assets/94988259-0461-44de-b7ad-c5a0027821a9)

Step 2 :  Secure Apache with a Firewall, Because it will Blocks unauthorized access to my server.

![ufw configuration   start apache2](https://github.com/user-attachments/assets/2917daef-2796-48d2-a045-b58855549541)

Step 3 : Disable Directory Listing, first we will Open the Apache configuration file and Find the <Directory> section and change Options Indexes to Options -Indexes:
Why: Prevents hackers from browsing your files.

![Hide Apache Version and OS Info](https://github.com/user-attachments/assets/1a280ae3-0b2a-427c-914b-10ccae359e97)

![directory change](https://github.com/user-attachments/assets/d933fda5-75af-4d3b-8a94-f261f1d9d49c)

Step 4 : 5. Hide Apache Version and OS Info, and Open the security configuration file and Change these lines: ServerTokens Prod
ServerSignature Off.
Why: Prevents hackers from knowing your server’s software and version.

![Hide Apache Version and OS Info](https://github.com/user-attachments/assets/528d9f5b-d1ea-4a3a-9189-ab67d5dc4e64)

Step 5 : ModSecurity (Web Application Firewall), and we will install Modsecurity and enable and configure it, Then restart the apache2.
Why: Blocks common web attacks like SQL injection.

![Use ModSecurity](https://github.com/user-attachments/assets/09c18b51-eb04-499a-89ca-ebd305399e15)

![enabling mod security](https://github.com/user-attachments/assets/995e4cfb-2f2f-46c4-b540-c1976a7d6146)

Step 6 :  HTTPS (SSL/TLS), and Install Certbot and encrypt the web server Using SSL certificate, and we have to Follow the prompts to secure domain.
Why: Encrypts data between your server and users.

![ssl and tls](https://github.com/user-attachments/assets/13b1e126-de4e-4b01-a479-aff070c990ae)

![SSL certificate](https://github.com/user-attachments/assets/b73e68be-f472-4355-add9-94287cf3cec7)

Step 7 : Regularly Monitor Logs, and check apache logs. 
Why: Helps detect suspicious activity.

![Regularly Monitor Logs](https://github.com/user-attachments/assets/4c81996a-fb68-479a-bdff-ec3ce9fd0881)













