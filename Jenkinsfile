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
        sh 'mvn verify'
      }
    }

  }
  tools {
    maven 'MVN'
    jdk 'Java'
  }
}