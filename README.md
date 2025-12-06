
# SonarQube Terminal Demo Guide

## Step 1 — Clone Sample Repository
```
git clone https://github.com/SonarSource/sonar-scanning-examples.git
cd sonar-scanning-examples/sonarqube-scanner/src
```

## Step 2 — Install SonarScanner
```
wget https://binaries.sonarsource.com/Distribution/sonar-scanner-cli/sonar-scanner-6.0.0.4432-linux.zip
unzip sonar-scanner-*.zip
sudo mv sonar-scanner-* /opt/sonar-scanner
export PATH=$PATH:/opt/sonar-scanner/bin
```

## Step 3 — Create Project in SonarQube
- Create new project
- Get project token

## Step 4 — Add sonar-project.properties
```
sonar.projectKey=demo-project
sonar.projectName=Demo Project
sonar.projectVersion=1.0
sonar.sources=.
sonar.java.binaries=.
sonar.host.url=http://localhost:9000
sonar.login=YOUR_TOKEN_HERE
```

## Step 5 — Run Scan
```
sonar-scanner
```
