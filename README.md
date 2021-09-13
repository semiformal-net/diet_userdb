# Diet user management

This is a flask frontend for user registration and login. It uses Oauth from google (sorry). It closely follows this [example](https://realpython.com/flask-google-login/)

# Setup

1. You need to make OAuth credentials for google. In the GCP project for this app, follow [these steps](https://realpython.com/flask-google-login/#creating-a-google-client). Be sure to put in your email as a test user.

# Environment

See `requirements.txt`

To run properly the app expects to secrets to be available as environment variables, `GOOGLE_CLIENT_ID` and `GOOGLE_CLIENT_SECRET`. You need those from the [GCP console](https://console.cloud.google.com/apis/credentials) of your OAuth client IDs. And then,

```
export GOOGLE_CLIENT_ID=blahblahblah.apps.googleusercontent.com
export GOOGLE_CLIENT_SECRET=blahblahblah
python app.py 
```