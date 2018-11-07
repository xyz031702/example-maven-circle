# Black Duck CoPilot Maven/Circle CI Example

[![CircleCI](https://img.shields.io/circleci/project/github/BlackDuckCoPilot/example-maven-circle/master.svg)](https://circleci.com/gh/BlackDuckCoPilot/example-maven-circle) [![Black Duck Security Risk](https://copilot.blackducksoftware.com/github/repos/BlackDuckCoPilot/example-maven-circle/branches/master/badge-risk.svg)](https://copilot.blackducksoftware.com/github/repos/BlackDuckCoPilot/example-maven-circle/branches/master)

Shows a working setup for using Black Duck CoPilot to analyze the risk of project dependencies

## Circle CI Setup

The `circle.yml` file has been modified to upload the generated data to Black Duck CoPilot:

```yaml
    - deploy:
          command: bash <(curl -s https://copilot.blackducksoftware.com/ci/circle2/scripts/upload)
```
