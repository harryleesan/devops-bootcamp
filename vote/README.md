# Voting app

## Introduction
Dockerise a Python application to track votes in Redis.

## Task
- Create 2 docker containers, one will be running Redis and the other will be
  running the python application. (Bonus if you can get _docker-compose_ right).
- This means that you need to create at least one Dockerfile to package the python
  application.

## Running the voting app
Steps to run the application:
1. Ensure that **Python 2.7** is installed.
2. `pip install -r requirements.txt`
3. `python app.py`
4. The app should now be accessible at `http://localhost:5000`.

## Testing the results in Redis
[Redis](https://redis.io/) is used as a queue to store all votes from the Python application. To test
if the Python application is persisting to Redis, follow the below steps.
1. Vote on the Python application.
2. Connect to Redis.
3. Execute `keys *`, you should be able to see a "votes" document.

