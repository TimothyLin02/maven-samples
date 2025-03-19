pipeline {
  agent any
  tools { 
      maven 'MVN' 
      jdk 'Java' 
  }
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
}
