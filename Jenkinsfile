pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            echo 'Building the Spring Boot basic application'
          }
        }

        stage('Test') {
          steps {
            echo 'Testing the application'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploying the Application in server'
      }
    }

  }
  // environment {
  //   DummyChromeDriverVersion = 'ChromeDriver 114.0.5735.90'
  // }
}