#!groovy
node {
  stage('Get Repository'){
    checkout scm
  }
  stage('Clean'){
    sh('mvn clean')
  }
  stage('Build'){
    sh('chmod +x mvnw')
    sh('./mvnw')
  }
  stage('Report'){
    echo currentBuild.durationString
  }
}
