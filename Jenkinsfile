pipeline {
  agent any
  stages {
    stage('---clean---') {
      parallel {
        stage('---clean---') {
          steps {
            bat 'mvn clean'
          }
        }
        stage('loli') {
          steps {
            bat 'jar -version'
          }
        }
      }
    }
    stage('--test--') {
      steps {
        bat 'mvn test'
      }
    }
    stage('--package--') {
      steps {
        bat 'mvn package'
      }
    }
  }
}