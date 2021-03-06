# TVVS Static Analysis
FEUP TVVS Static Analysis Lecture

This project has the proposal to show SonarLint and SonarCloud working with Intellij and Github Actions to review the code for a small Java H2 example.

[![Vulnerabilities](https://sonarcloud.io/api/project_badges/measure?project=kadubarral_tvvs-staticanalysis&metric=vulnerabilities)](https://sonarcloud.io/dashboard?id=kadubarral_tvvs-staticanalysis)
[![Bugs](https://sonarcloud.io/api/project_badges/measure?project=kadubarral_tvvs-staticanalysis&metric=bugs)](https://sonarcloud.io/dashboard?id=kadubarral_tvvs-staticanalysis)
[![Code Smells](https://sonarcloud.io/api/project_badges/measure?project=kadubarral_tvvs-staticanalysis&metric=code_smells)](https://sonarcloud.io/dashboard?id=kadubarral_tvvs-staticanalysis)
[![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=kadubarral_tvvs-staticanalysis&metric=sqale_rating)](https://sonarcloud.io/dashboard?id=kadubarral_tvvs-staticanalysis)
[![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=kadubarral_tvvs-staticanalysis&metric=security_rating)](https://sonarcloud.io/dashboard?id=kadubarral_tvvs-staticanalysis)

![Unit Test](https://github.com/kadubarral/tvvs-staticanalysis/workflows/Build/badge.svg)

## Setup Activities
Fork this project
![PR](docs/github-FORK.png)

Clone the project that you forked
```shell script
git clone https://github.com/YOUR_NAME/tvvs-staticanalysis.git
```

Branch
```shell script
git checkout main
git pull upstream main && git push origin main
git checkout -b upXXXXXXXXX/static-analysis-fix
```

## Fix the issues
Work in your machine
```shell script
cd tvvs-staticanalysis
```

Static Test is not about to execute the code, but if you want to run locally you can use maven.
```shell script
mvn clean compile exec:java
```

#### To help your work
* See the actual report of issues on SonarCloud
    * https://sonarcloud.io/dashboard?id=kadubarral_tvvs-staticanalysis
* Use SonarLint report on Intellij 

## Send your code
Commit and push
```shell script
git add -A
git commit -m "fix a lot of issues in this horrible code"
git push origin upXXXXXXXXX/static-analysis-fix
```

Create the PR
![PR](docs/github-PR.png)

### Group Members
* Kadu Barral
* Sadra Farshid