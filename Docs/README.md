# Udagram

## Description

**udagram is fullstack application build in Angluar and nodejs**

provided by udacity to be hosted in AWS with pipeline using CircleCi

**The Project is for the Advanced Full-Stack Web Development Nanodegree Program**

built with :->

-   [Angular](https://angular.io/) - Single Page Application Framework
-   [Node](https://nodejs.org/) - Javascript Runtime
-   [Express](https://expressjs.com/) - Javascript API Framework

### Dependencies

```
- Node v14.15.1 (LTS) or more recent. While older versions can work it is advisable to keep node to latest LTS version

- npm 6.14.8 (LTS) or more recent, Yarn can work but was not tested for this project

- AWS CLI v2, v1 can work but was not tested for this project

- A RDS database running Postgres.

- A S3 bucket for hosting uploaded pictures.
```

### AWS Cloud setup

-   RDS - database name : udagram
-   RDS - database port : 5432
-   RDS - Database Host : database-1.c821gx45oq5b.us-east-1.rds.amazonaws.com
-   frontend - S3 : http://udagramzbucket.s3-website-us-east-1.amazonaws.com
-   EB url / api link : http://udagram-api-dev.eba-v3qbepu3.us-east-1.elasticbeanstalk.com/

### Environment Variables

in .env file or in Cloud env

```
- PORT                = 3000
- POSTGRES_HOST       = <Database_IP_Address>
- POSTGRES_PORT       = <Database_Port>
- POSTGRES_DB         = <Database_Name>
- POSTGRES_USERNAME   = <Database_Username>
- POSTGRES_PASSWORD   = <Database_Password>
- URL                 = <Url>
- JWT_SECRET          = <Any_PassPhrase>
- AWS_REGION          = <us-east-1>
- AWS_PROFILE         = <Profile>
- AWS_BUCKET          = <Bucket_Name>

```

### Pipeline

```
- `npm run frontend:install`    - To install frontend dependencies.
- `npm run frontend:build`      - To build the Angular/Frontend.
- `npm run frontend:deploy`     - To deploy the project to S3 using `./udagram-frontend/bin/deploy.sh` deploy script.
- `npm run backend:install`     - To install backend dependencies.
- `npm run backend:build`       - To transpile the Typescript/Backend.
- `npm run backend:deploy`      - To deploy the project to EB using `./udagram-api/bin/deploy.sh` deploy script.
```
