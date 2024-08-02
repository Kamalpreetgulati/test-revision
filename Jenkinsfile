pipeline {
    agent any
    stages {
        stage('Fetch Code') {
            steps {  // Change 'step' to 'steps'
               git branch: 'main', url: 'https://github.com/Kamalpreetgulati/test-revision.git'
            }
        }
        stage('Install Webserver') {
            steps {  // Change 'step' to 'steps'
               sh 'sudo apt install apache2 -y'
            }
        }
        stage('Deploy Application') {
            steps {  // Change 'step' to 'steps'
               sh 'sudo cp -R * /var/www/html/'
            }
        }
    }
}
