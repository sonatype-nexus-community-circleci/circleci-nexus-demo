# CircleCI 2.1 example publishing To Nexus Repository Manager
[![CI](https://circleci.com/gh/sonatype-nexus-community-circleci/circleci-nexus-demo.svg?style=shield&circle-token=:circle-token)](https://circleci.com/gh/sonatype-nexus-community-circleci/circleci-nexus-demo)
[![CI](https://circleci.com/gh/collinpeters/circleci-nexus-demo.svg?style=shield&circle-token=:circle-token)](https://circleci.com/gh/collinpeters/circleci-nexus-demo)

This is an example application showcasing how to deploy a Java app to Sonatype Nexus Repository Manager via CircleCI 2.1.

This application uses the following tools: 

* Sonatype Nexus Repository Manager 
* Maven 
* Java 8 
* PostgreSQL 
* Spring 
* Thymeleaf

## Sonatype Nexus Repository Manager
You can use your existing Nexus Repository Manager instance (must be accessible to CircleCI), or for testing see the instructions [here](https://help.sonatype.com/display/NXI/CloudFormation+-+Repository+Manager) to stand up a test Nexus Repository Manager instance on AWS.

## Circle CI
I would recommend to fork this repository, update the path to your Repository Manager instance, and then build this repository in CircleCI.

The original sample Java application is documented [here](https://circleci.com/docs/2.0/language-java/).

## Notes
For ease of use the sample CircleCI [config.yml](.circleci/config.yml) hard-codes the Nexus Repository Manager username, password, and server url. Outside of testing you should not hard code these values into your configuration, but rather use environment variables as described [here](https://github.com/sonatype-nexus-community/circleci-nexus-orb#circleci-context-support)

## License

Copyright © 2017 CircleCI

Distributed under the MIT license, see the file LICENSE.

