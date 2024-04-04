# awssesh

A simple interactive CLI utility to work with AWS session manager.

## Prerequisites

bash
aws cli - https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html
aws session manager plugin - https://docs.aws.amazon.com/systems-manager/latest/userguide/session-manager-working-with-install-plugin.html
jq - https://jqlang.github.io/jq/download/

## Usage

awssesh [-p aws profile name] [-i instance tag]

## Configuration

Configuration can be provided by command line flags, via interactive prompt or via environment variables.

Environment variables used to configure awssesh

    export AWS_PROFILE="myProfileName"
    export INSTANCE_TAG="myTag"