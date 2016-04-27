
# Autoscaling

Create an autoscaling setup with the template autoscaling.json. Find a way to put load on the system and watch what happens.

# Creating the stack

Create the example stack with this command:

```
aws cloudformation create-stack --stack-name autoscaling template-body file://./autoscaling.json
```

Note: The required parameters can be passed with ```--parameters  ParameterKey=KeyPairName,ParameterValue=MyKey ```

# Deleting the stack

You can delete the stack with this command:

```
aws cloudformation delete-stack --stack-name autoscaling
```

# Updating the stack

You can update the stack with this command:

```
aws cloudformation update-stack --stack-name autoscaling --template-body file://./autoscaling.json
```
