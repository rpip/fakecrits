## fakecrits

script to load some fake data into CRITs

### setup
* Enable the API
* RUN `$ ./fakecrits --url=https://localhost:8443/ --user=nonroot --key=7503c6ce486dbe91fd94315eb64374681661428d`
* subscribe to the source. The default source is `Faker Vault`.

    If necessary, add a source to CRITs for AlienVault. To do this:

    1. Click the gear symbol in the top left and go to "CRITs Control Panel".
    2. Click "Items" then the "Sources" tab.
    3. Click "Add SourceAccess" near the top right. Add your source.
    4. Go to the "Users" section on the left hand side.
    5. Allow the user to use the source.

* More

``` shell
λ ./fakecrits -h
usage: fakecrits [-h] --url URL --user USER --key KEY [--source SOURCE]
                 [--campaign CAMPAIGN] [-v]

Imports fake data into CRITs

optional arguments:
  -h, --help           show this help message and exit
  --url URL
  --user USER
  --key KEY
  --source SOURCE
  --campaign CAMPAIGN
  -v                   verify HTTPs endpoint
```

## similar tools

* Pulls actual data (indicators and events) from subscribed Alienvault OTX pulses https://github.com/lolnate/otx2crits
