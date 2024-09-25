Scalable Journalling App -->using Kafka, Redis, MongoDB, jwt, and cron jobs. 
Admin can create new admin users.
Admin     can view all users

User---->will log in to  see the welcome message with weather fetched from the external API
the request will check the Redis cache before fetching data from the external API

User--------> can  CRUD journal entry.
User -------->can subscribe to journal application sentiment analysis service 
CRON job will run fetching sentiment reports of the journal for each user to send mail to all users who have subscribed
sentiment job will communicate with email asynchronously service via Kafka

Logs will 

@mockito used for testing
Mongodb as db
JWT for authentication and authorization

The sentiment analysis  service is a mock service for now
