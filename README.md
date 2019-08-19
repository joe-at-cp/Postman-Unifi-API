# Postman-Unifi-API-
Ubiquiti Unifi API - Postman Collection File

A Simple Postman Collection file to interact with Ubiquiti Unfi Controllers and Sites using a REST API. 

For the Postman Environment, create the following variables for the collection:
1) "controller" - This is the URL and port to your Unifi Controller (example value: "https://192.168.1.100:8443")
2) "site" - This is the Unifi site name as configured in the Unifi Controller. If you are unable to find the site name you can issue the "self sites" api call to get a list of configured sites and their names (example value: default)

Unifi API Flow: 
1) Login -> Upon successful login your client will recieve a token cookie (Postman automatically saves these cookies)
2) Execute any api call as long as your cookie is still valid. Keep in mind that some api calls will not work unless your api user account has read/write privledges.
