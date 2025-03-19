pipeline {
  agent any
  tools { 
      maven 'Maven' 
      jdk 'JAVA' 
  }
  stages {
    stage('check out') {
      steps {
        git(url: 'https://github.com/joycedaiyt/maven-samples', branch: 'master')
      }
    }

    stage('run') {
      steps {
        sh 'mvn verify'
      }
    }

  }
}