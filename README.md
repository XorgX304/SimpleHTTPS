# SimpleHTTPS
    Quick and dirty HTTPS Python Server.

# Usage:
     1. Define server IP Address and Port
        python simplehttps.py --server 127.0.0.1 --port 443
   
     2. Create Self Signed Cert
        Set up a new PEM password, enter Country Name, State, etc ..
     
     3. Start HTTPS Server
        Enter your previous PEM password to start HTTPS server.
     
     Note: HTTPS server runs in SimpleHTTPS/var/www/


    Example:
         SimpleHTTPS v1.05012017
         Description: Quick and dirty HTTPS Python Server.
         Created by: Nick Sanzotta/@Beamr
         *******************************************************************************
         openssl req -nodes -x509 -newkey rsa:2048 -keyout ../../key.pem -out ../../cert.pem -days 365 -subj                            "/C=US/ST=DEL/L=DOVER/O=Company Inc/OU=IT/CN=www.test.com/emailAddress=it@support.com"
         
         Generating a 2048 bit RSA private key
         .......+++
         ........................................+++
         writing new private key to '../../key.pem'
        -----
         [i] SSL Certificate Created:
         [i] HTTPS Server Started: https://127.0.0.1:443
        ----------------------------------------

# Help
    optional arguments:
      -h, --help            show this help message and exit

    Server options:
      -s Default [127.0.0.1], --server Default [127.0.0.1]
      -p [Default [443]], --port [Default [443]]

    SSL Cert options:
      -cn Default [US], --country Default [US]
      -st Default [DEL], --state Default [DEL]
      -c Default [DOVER], --city Default [DOVER]
      -comp Default [Company Inc], --company Default [Company Inc]
      -ou Default [IT], --orgUnit Default [IT]
      -d Default [www.myserver.com], --fqdn Default [www.myserver.com]
      -e Default [it@support.com], --email Default [it@support.com]



 
 
