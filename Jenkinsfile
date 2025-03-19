pipeline {
  agent any
  stages {
    stage('check out') {
      steps {
        git(url: 'https://github.com/TimothyLin02/maven-samples.git', branch: 'master')
      }
    }

    stage('run') {
      steps {
        sh 'mvn test'
        sh 'mvn verify'
        sh 'mvn clean'
      }
    }

  }
  tools {
    maven 'MVN'
    jdk 'Java'
  }
}