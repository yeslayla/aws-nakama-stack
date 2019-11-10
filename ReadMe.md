# Heroic Lab's Nakama on ECS

CloudFormation stack for creating an ECS service for Nakama.

## Launching Stack

Make sure you are logged into the AWS Console and have permissions then click:

[![Launch Stack](https://cdn.rawgit.com/buildkite/cloudformation-launch-stack-button-svg/master/launch-stack.svg)](https://console.aws.amazon.com/cloudformation/home?region=us-east-1#/stacks/create/template?stackName=Nakama&templateURL=https://sumu-stacks.s3.amazonaws.com/nakama/production/cloudformation/nakama/top.yaml)

Fill out the parameters and launch!

### Parameter Notes

Parameters, `DatabaseUsername`, `DatabasePassword`, `DatabaseEndpoint`, and `DatabasePort`, only used if `CreateDatabase` is false.

## To Do

- [x] Load Balancing
    - [ ] [Clustering](https://heroiclabs.com/nakama-enterprise/)
- [ ] Auto Scaling
- [x] Dynamic Port Routing
- [x] HTTPS
- [x] Build Database
    - [ ] Database configuration
    - [x] Automatically migrate database
- [x] Custom Admin User
- [ ] Custom security keys
- [ ] Formatted Launch Parameters
- [ ] Informative `ReadMe.md`
- [ ] Load Server Modules
