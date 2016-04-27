
# Relations for JIRA stack

The relations.json file is almost all of our production stack. Do a walkthrough. Do you recognize all the component from the presentation? If you feel really brave today, try creating the stack and see how far you get. You may be missing stuff, you may need my help.

Tip: Start with some real simple components, like for example the S3 buckets. Make a copy of the file and gradually add components. You may want to skip the Transactor layer, or pick another image instead of the datomic one. Also, take a look at the UserData parts and ditch what you don't need.

# Creating the stack

Create the example stack with this command:

```
aws cloudformation create-stack --stack-name relations template-body file://./relations.json
```

Note: The required parameters can be passed with ```--parameters  ParameterKey=KeyPairName,ParameterValue=MyKey ```

# Deleting the stack

You can delete the stack with this command:

```
aws cloudformation delete-stack --stack-name relations
```

# Updating the stack

You can update the stack with this command:

```
aws cloudformation update-stack --stack-name relations --template-body file://./relations.json
```
