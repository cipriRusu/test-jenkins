pipeline {
    agent {
        docker { image 'ubuntu:20.04' } 
    }

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                sh 'curl -sL https://deb.nodesource.com/setup_14.x | sudo -E bash -'
                sh 'sudo apt-get install -y nodejs'
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