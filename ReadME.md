Scalable Journalling App

User---->will log in to  see the welcome message with weather fetched from external api
request will check redis cache before fetching data from exteranal api

User--------> can  CRUD journal
User -------->can subscribe to journal application sentimentAnalysis service 
CRON job will run fetching sentiment reports of journal for each user to send mail to all users who have subscribed
sentiment job will communicate with email asynchronously service via kafka

Logs will 

@mockito used for testing
Mongodb as db
JWT for authentication and authorization

The sentiment analysis  service is a mock service for now
