# Amazon Route53 Dynamic DNS Updater

This project leverages the Amazon Route53 API to provide a dynamic DNS service through A (alias/subdomain) records.

## Setup
As indicated by the Area53 documentation, users need to set the following environment variables:

```bash
export AWS_ACCESS_KEY_ID="<Insert your AWS Access Key>"
export AWS_SECRET_ACCESS_KEY="<Insert your AWS Secret Key>"
```

before a connection can be made.

## Use
```r53dyndns.py --record=RECORD_TO_UPDATE --url=IP_GET_URL```

## Dependencies :

+   A URL that returns the client IP alone in plaintext. No support is included for other standard services.
+   Area53 interface : https://github.com/bigmlcom/Area53
+   boto : https://github.com/boto/boto
