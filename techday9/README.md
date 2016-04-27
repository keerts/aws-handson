
# Elastic Beanstalk

Deploy an existing (Java?) application using Elastic Beanstalk. The eb.json file contains an example with php. I'm sure you are capable of turning this into an example that uses one of your existing apps. 

# Creating the stack

Create the example stack with this command:

```
aws cloudformation create-stack --stack-name eb --template-body file://./eb.json
```

You can delete the stack with this command:

```
aws cloudformation delete-stack --stack-name eb
```

You can update the stack with this command:

```
aws cloudformation update-stack --stack-name eb --template-body file://./eb.json
```

# Tips for the wrapup!

Present to us:

* How does this compare to running an app on EC2? 
* Does it make your life easier?
* How does it compare to AWS Lambda.
