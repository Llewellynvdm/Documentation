# REST API: GET statistics (Marketing Suite mailing)

You can retrieve the statistics of a Marketing Suite mailing by sending an HTTP GET request to the following URL:

`https://api.copernica.com/v2/ms/emailing/$id/statistics?access_token=xxxx`

Where the `$id` should be replaced with the ID of the mailing.

## Available parameters

* **begintime**: Start date (and time) for the statistics.
* **endtime**: End date (and time) for the statistics.

## Returned fields

The **data** field of returned JSON object contains the statistics. 
The following fields are available:

* **destinations**: The number of destinations for this mailing.
* **abuses**: The number of abuses for this mailing.
* **clicks**: An array with fields 'total' and 'unique' for the total 
number of clicks and number of unique clicks respectively.
* **deliveries**: The number of deliveries for this mailing
* **errors**: The number of errors for this mailing.
* **impressions**: An array with fields 'total' and 'unique' for the 
total number impressions and number of unique impressions respectively.
* **retries**: The number of retries for this mailing.
* **unsubscribes**: The number of unsubscribes for this mailing.

## PHP example

This script demonstrates how to use this API method:

```php
// dependencies
require_once('copernica_rest_api.php');

// change this into your access token
$api = new CopernicaRestAPI("your-access-token", 2);

// execute the call
print_r($api->get("ms/emailing/{$emailingID}/statistics/"));
```

This example requires the [REST API class](./rest-php).

## More information 

* [Overview of all REST API calls](./rest-api)
* [Retrieve a Marketing Suite emailing](./rest-get-ms-emailing)
