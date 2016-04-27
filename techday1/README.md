
# Notarisnet

Bouw Notarisnet door middel van Cloudformation. Ik heb een voorbeeld-template van een stack bijgevoegd als inspiratie.

# Creating the stack

Create the example stack with this command:

```
aws cloudformation create-stack --stack-name notarisnet --template-body file://./notarisnet.json
```

You can delete the stack with this command:

```
aws cloudformation delete-stack --stack-name notarisnet
```

You can update the stack with this command:

```
aws cloudformation update-stack --stack-name notarisnet --template-body file://./notarisnet.json
```

# Tip!

Kijk ook eens naar CloudFormer. Wellicht kun je Hiermee een template maken voor een bestaande configuratie?
