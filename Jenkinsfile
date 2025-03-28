pipeline {
    agent any
    tools {
        nodejs 'NodeJS_14.17.1'
    }

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                sh 'npm install typescript'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}