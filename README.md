# How to Upload Any Type of Binary File to S3 via API Gateway

## Upload any type of file to the S3 bucket using Lambda proxy integration with API Gateway in Python


### Prerequisite
- Node
- Serverless Framework must be installed on your machine

**Follow the below steps to deploy this small module to AWS Cloud** 

1. Clone this repo.
2. Install dependencies using `npm install`.
3. Create config file with this name `config.stage.json`. Stage will be your appication stage e.g. `dev`, `test` or `prod`.
4. Write unique name of your bucker in config file.
    * The following rules apply for naming buckets in Amazon S3
        - Bucket names must be between 3 and 63 characters long.
        - Bucket names can consist only of lowercase letters, numbers, dots (.), and hyphens (-). 
        - Bucket names must begin and end with a letter or number.
        - Bucket names must not be formatted as an IP address (for example, 192.168.5.4). 
        - Bucket names must not start with the prefix `xn--`.

At the end run the below command.
```
serverless deploy
```

**Follow the below steps to remove this small module from AWS Cloud** 

1. First, empty your s3 bucket from console.
2. Go to the inside of your project folder on your machine.

And run the below command.
```
serverless remove
```
