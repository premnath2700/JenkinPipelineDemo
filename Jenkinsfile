pipeline {
  agent any
  stages {
    stage('checkout') {
      steps {
        git 'https://github.com/premnath2700/SpringBootJenkinsDemo.git'
      }
    }
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
      when {
        branch 'main'
      }
      steps {
        echo 'Deploying the Application in server'
      }
    }

  }
}