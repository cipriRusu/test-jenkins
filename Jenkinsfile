pipeline {
    agent {
        docker { image 'ubuntu:20.04' } 
    }

    stages {
        stage('Install Node.js and npm') {
            steps {
                script {
                    sh '''
                    curl -fsSL https://deb.nodesource.com/setup_14.x | sudo -E bash -
                    sudo apt-get install -y nodejs
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