pipeline {
    agent any

    tools {
        maven 'maven'  // Name must match your Maven installation in Jenkins
    }

    stages {
        stage('Build') {
            steps {
                git credentialsId: 'e4fc89ca-ddd7-4094-8a90-452c4546dac9', url: 'https://github.com/PALLAVI-96/java-hello-world-with-maven.git'
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
