pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
	      sh 'mvn clean install'
            }

        }
        stage('Test') {
            steps {
                echo 'Testing..'
                sh 'mvn test'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
                sh 'mvn deploy'
            }
        }
    }
}
