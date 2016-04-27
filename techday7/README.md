
# Static website

Host a static website on S3. It's that simple.

# Creating the stack

Create the example stack with this command:

```
aws cloudformation create-stack --stack-name static template-body file://./static.json
```

Note: The required parameters can be passed with ```--parameters  ParameterKey=KeyPairName,ParameterValue=MyKey ```

# Deleting the stack

You can delete the stack with this command:

```
aws cloudformation delete-stack --stack-name static
```

There is something special to the deletion for this stack, can you spot it?

# Updating the stack

You can update the stack with this command:

```
aws cloudformation update-stack --stack-name static --template-body file://./static.json
```

# Tips for the wrap-up

Present to us:

* How cheap is it to host a static website on S3?
* What other services can be combined with S3?
* How about ssl?
* Show me the website!
