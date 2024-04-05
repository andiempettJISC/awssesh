# awssesh

A simple interactive CLI utility to work with AWS session manager.

## Prerequisites

bash
aws cli - https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html
aws session manager plugin - https://docs.aws.amazon.com/systems-manager/latest/userguide/session-manager-working-with-install-plugin.html
jq - https://jqlang.github.io/jq/download/

## Install

```shell
brew tap andiempettJISC/awssesh
brew update
brew install awssesh
```

## Usage

    awssesh [-p aws profile name] [-i instance tag]

## Configuration

Configuration can be provided by command line flags, via interactive prompt or via environment variables.

Environment variables used to configure awssesh

    export AWS_PROFILE="myProfileName"
    export INSTANCE_TAG="myTag"

AWS_PROFILE = the AWS credentials profile to use listed in ~/.aws/config. This must be configured first

INSTANCE_TAG = a fuzzy search for a tag assigned to an EC2 instance. Used to filter the list of instances