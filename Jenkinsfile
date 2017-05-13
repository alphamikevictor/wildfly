#!groovy
node {
  stage('Get Repository'){
    checkout scm
  }
  stage('Clean'){
    sh('mvn clean')
  }
  stage('Build'){
    sh('mvn')
  }
  stage('Report'){
    echo currentBuild.durationString
  }
}
