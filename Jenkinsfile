pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'mvn clean'
      }
    }
    stage('Test') {
      steps {
        sh 'mvn test'
      }
    }
    stage('Deploy') {
      steps {
        sh 'mvn package'
      }
    }
    stage('report') {
      steps {
        echo 'reporting'
        //cucumber fileIncludePattern: '**/*.json', sortingMethod: 'ALPHABETICAL'
      }
    }
  }
}
