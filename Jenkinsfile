pipeline {
  agent any
  stages {
    stage('Sonarqube Analysis') {
      steps {
        withSonarQubeEnv('static') {
          sh './mvnw clean package sonar:sonar'
        }
      }
    }
  }
}
