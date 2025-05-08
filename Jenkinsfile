pipeline {
    agent any

    tools {
        maven 'maven-3.8'  // Name must match your Maven installation in Jenkins
    }

    stages {
        stage('Build') {
            steps {
                sh 'mvn clean install'
            }
        }

        stage('Test') {
            steps {
                sh 'mvn test'
            }
        }
    }
}
