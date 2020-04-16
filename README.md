# React Video Twilio App
Twilio React Video app
## Getting Started
```
node version > 10.6
postgresql
```
### Installing
```
npm install
```

### Configure credentials

make .env file
```
cp .env.examle .env
```

Twilio account credentials
```
TWILIO_ACCOUNT_SID=YOUR_ACCOUNT_SID
TWILIO_API_KEY_SID=YOUR_PROJECT_API_KEY
TWILIO_API_KEY_SECRET=YOUR_PROJECT_API_SECRET
```
To learn more about how to get credentials, visit here

https://www.twilio.com/docs/video/tutorials/user-identity-access-tokens

### Create database and connect to db
configure postgresql database
```
# POSTGRES DATABASE CREDNETIALS
POSTGRES_USERNAME=
POSTGRES_PASSWORD=
POSTGRES_HOST=
POSTGRES_PORT=
POSTGRES_DBNAME=
```

user table schema
```
CREATE TABLE public.users (
    accesscode character varying(100),
    username character varying(100),
    roomname character varying(100)
);
```

sample database file
```
dump.sql
```

### Run
```
npm start
```

