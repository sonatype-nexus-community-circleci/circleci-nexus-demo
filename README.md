# CircleCI publishing To Nexus Repository Manager

This is an example application showcasing how to deploy a Java app to Sonatype Nexus Repository Manager via CircleCI 2.1.

The following tools are used:

* Sonatype Nexus Repository Manager
* Maven
* Java 8
* PostgreSQL
* Spring
* Thymeleaf

## Sonatype Nexus Repository Manager
You can use your existing Nexus Repository Manager instance (must be accessible to CircleCI), or for testing see the instructions [here](https://help.sonatype.com/display/NXI/CloudFormation+-+Repository+Manager) to stand up a test Nexus Repository Manager instance on AWS.

## Circle CI
To test this application in CircleCI, fork this repository, and set the following build variables in CircleCI:
* NEXUS_RM_USERNAME - Username to access Nexus Repository Manager
* NEXUS_RM_PASSWORD - Password to access Nexus Repository Manager
* NEXUS_RM_SERVERURL - Nexus Repository Manager Server URL

## Notes
* The original sample Java application by CircleCI is documented [here](https://circleci.com/docs/2.0/language-java/).
* For ease of use the sample CircleCI [config.yml](.circleci/config.yml) hard-codes the Nexus Repository Manager username, password, and server url. Outside of testing you should not hard code these values into your configuration, but rather use environment variables as described [here](https://github.com/sonatype-nexus-community/circleci-nexus-orb#circleci-context-support)

## License

Copyright © 2017 CircleCI

Distributed under the MIT license, see the file LICENSE.
