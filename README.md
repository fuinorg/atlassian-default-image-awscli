# atlassian-default-image-awscli
The [Atlassian default build environment Docker image](https://hub.docker.com/r/atlassian/default-image/) for Bitbucket Pipelines *plus* the AWS Command Line Interface (CLI).

[![Automated Docker Build](https://img.shields.io/docker/automated/fuinorg/atlassian-default-image-awscli.svg)](https://hub.docker.com/r/fuinorg/atlassian-default-image-awscli/)

## Versions

- atlassian/default-image:1.70

## Usage

Simply use this image in your 'bitbucket-pipelines.yml' file:

    image: fuinorg/atlassian-default-image-awscli:latest
    pipelines:
      default:
        - step:
            script:
              - aws codebuild start-build --project-name "<your-project-name>"

Above configuration is an example on how to start an AWS CodeBuild using the Bitbucket pipeline. 
