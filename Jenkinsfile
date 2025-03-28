pipeline {
    agent {
        docker { image 'ubuntu:20.04', args '--user root' }
    }

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                sh '''
                    apt-get update || true
                    apt-get install -y sudo curl
                    curl -fsSL https://deb.nodesource.com/setup_14.x | bash -
                    sudo apt-get install -y nodejs npm
                    '''
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