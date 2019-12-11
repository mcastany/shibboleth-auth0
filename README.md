## README

This is just a PoC on how to integrate Auth0 as an IDP and Shibboleth SP

1. Signup in Auth0

1. Create a new application

1. In the addons section, click on the SAML addon

1. Configure `Application Callback URL` with the following value

```
https://${DOMAIN}/Shibboleth.sso/SAML2/POST
```

1. Update the .env file with the appropiate values

1. Go to the terminal and run

```
docker-compose up -d
```

1. Navigate to `https://{HOSTNAME}`
