### My experiments based on the FEM course
* vanilla setup:
* $ npm i -g serverless
* $ sls --help
* $ sls create -t aws-nodejs -p demo-sls


### invoke handler fn locally (from within folder containing the handler fn)
* $ sls invoke local -f hello
* $ sls invoke local -f test1
* $ sls invoke local -f todo

# testing routes
* $ sls offline start --port 4500
* $ http :4500/your_route

# run test2_9
* $ yarn dev
* or
* $ sls offline start --port 4500
* $ http :4500
* $ http :4500/todos
* $ http :4500/todo/1

# Deploy to lambda
> first configure serverless.yml file with service and profile... config
> be sure you are in the desired directory of the service you wish to deploy
* $ sls deploy

# Tailing the fn log
* $ sls logs -f <serviceName> -t

# Destroy a lambda
> this will destroy the target function
* $ sls remove

# Frontend Masters: [Serverless with AWS Lambda](https://frontendmasters.com/courses/serverless-aws/)
> Learn how to use AWS Lambda functions, by [Scott Moss](https://github.com/hendrixer)
> [github repo](https://github.com/FrontendMasters/serverless-with-aws) 

### tech check
* Node v8+
* Yarn / NPM (latest)

* Git + Github

## Course Format
This course has a video component on FrontEnd Masters. It follows the video closely. The repo is broken down into different branches in the following format:
`lesson-{lesson number}`
`lesson-{lesson-number}-solution`

## Get started
### AWS
You must have an AWS account for this to work. Don't worry, its free! After you have an account, you need to make a new user. Follow the instructions here: [Creating AWS Access Keys](https://serverless.com/framework/docs/providers/aws/guide/credentials#creating-aws-access-keys)
**Be sure** to setup your API credentials in your environment as well, [learn how](https://serverless.com/framework/docs/providers/aws/guide/credentials#using-aws-access-keys)

### Dependencies
* make sure to run `npm i` or `yarn` to install `node_modules`

