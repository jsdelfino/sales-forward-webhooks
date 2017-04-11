# sales-forward-webhooks

Samples shell scripts that call the Salesforce REST API used in the Watson
Workspace Sales Forward demo, using CURL.

To try them out do the following:

```
export SFDC_USER_ID=<your Salesforce user id>
export SFDC_PASSWORD=<your Salesforce password>
export SFDC_TOKEN=<your Salesforce token>
export SFDC_CONSUMER_KEY=<a Salesforce 'connected app' consumer key>
export SFDC_CONSUMER_SECRET=<a Salesforce 'connected app' consumer secret>

# Get an access token (saved in env var $SFDC_ACCESS_TOKEN)
. ./oauth

# Get lists of accounts, opportunities, contacts, and opportunity info
./accounts

./opportunities

./contacts "<account name>"

./opportunity "<opportunity name>"
```

