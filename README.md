# Hands on aws tech day

These are the hands on assignments for the AWS tech day on April 28 at Avisi.

If you weren't there, there might be not much use in this repository for you.

# Get started

1) Just log into the AWS console with the username/password and play around.
2) Install the CLI and follow the instructions

If you have questions, come to the HipChat room at: https://www.hipchat.com/gajDKStLg

(Avisi HipChat: AWS techday)

# Username / password

You have been given a user name / password that you can use to log into the AWS console. To log in, go to:

```
https://001194245973.signin.aws.amazon.com/console
```

# CLI

Install the command line interface.

OXS: brew install awscli
Arch Linux: https://aur.archlinux.org/packages/aws-cli/

General: http://docs.aws.amazon.com/cli/latest/userguide/installing.html

# Configure the CLI

You need to configure the CLI. The information you need is on your assignment sheet:

```
± |master ✗| → aws configure
AWS Access Key ID [None]: ******************
AWS Secret Access Key [None]: *************************************
Default region name [None]: us-east-1
Default output format [None]: json
```

NOTE: techday4, bij region, maak hier us-west-1 van!

For more information, or if you already have another account configured, see http://docs.aws.amazon.com/cli/latest/userguide/cli-chap-getting-started.html

# Look around on ec2 nodes

If you want to look around on EC2 nodes, create, or import an ssh key. You can do this in the console, or via the cli:

```
aws ec2 import-key-pair \
    --key-name ec2-$USER-key \
    --public-key-material  "$(ssh-keygen -y -f ~/.ssh/id_rsa)"
```

