pipeline {
    agent {
        docker { image 'node:14' }
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