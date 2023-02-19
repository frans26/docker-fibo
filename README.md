# docker-fibo

Sample project showcasing ability to develop multi-container application, docker multiple services, CI/CD using github actions and deploy multiple containers to AWS elasticbeanstalk 

## Applications

### client
Simple fibonacci calculator app. React application created using [create react app](https://github.com/facebook/create-react-app).

### server
Simple Express.js app handling post and get request for the client app. Used Redis for in-memory data storage and PostgreSQL for database.

### worker
Simple node.js app that watches redis for new index, calculates the fibonacci value by index and stores back again to redis.
