# Ticketnak

Project aimed to crawl Ticketswap listings on Facebook event and automatically opening the Ticketswap link in your browser
as soon as it's posted. This reserves the ticket for the user and is faster than refreshing on your own and clicking on the link.
Uses official Facebook API and doesn't crawl Ticketswap making it possible to run for hours in the background without 
getting blocked by Ticketswap.

The current interval is 2 seconds and I'm testing Facebook's request limit.

### Prerequisites

Runs on:

* Python=>3.0
* Python facebook-sdk

### Installing

```
git clone https://github.com/MartijnDevNull/ticketnak.git
```

```
cd ticketnak/src
```
```
virtualenv --python=/usr/bin/python3 env
```
```
pip install -r requirements.txt
```
```
cp facebook.ini-default facebook.ini
```
## Running

Make sure you have the configuration file (facebook.ini) setup with your Facebook event id. This can be found in the URL, for example:
* URL: https://www.facebook.com/events/285958198448885/
* Eventid: 285958198448885

Next create add your FB_APP_ID and FB_APP_SECRET found in [Facebook developer](https://developers.facebook.com/apps/) 

## Built With

* [Facebook SDK](https://github.com/mobolic/facebook-sdk) - Python SDK for Facebook's Graph API

## License

This project is licensed under the GPL v3 - see the [LICENSE](LICENSE) file for details