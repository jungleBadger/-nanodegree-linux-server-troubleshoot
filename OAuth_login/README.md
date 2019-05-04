# Error during Google OAuth login


### Issue description

Google OAuth failed to redirect or return unauthorized request or invalid_request


#### Debug

* Add site url `<Public_ip address>.xip.io` to *Authorised domains* field in     *OAuth consent screen*

* Add site url with http `http"//<Public_ip address>.xip.io` to *Authorized      JavaScript origins* in *Credentials Setting*

* Add redirect link to *Authorized redirect URIs* in *Credentials Setting*

* Download `client secret json` file and rename to `client_secrets.json`

* Replace the `client_secrets.json` file with the updated version in server

* Edit `flow_from_clientsecrets('client_secrets.json')` to `flow_from_clientsecrets('/var/www/<directory>/client_secrets.json')`

