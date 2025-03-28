pipeline {
    agent {
        docker { image 'ubuntu:20.04' } 
    }

    stages {
        stage('Install Node.js and npm') {
            steps {
                script {
                    sh '''
                    apt-get update
                    apt-get install -y curl sudo
                    curl -fsSL https://deb.nodesource.com/setup_14.x | bash -
                    apt-get install -y nodejs
                    '''
                }
            }
        }
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