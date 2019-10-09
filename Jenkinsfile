pipeline {
    agent {
        label 'windows && a102'
    }
    stages {
        stage('Build') {
            steps {
                bat 'echo "building"'
            }
        }
        stage('Bootload') {
            steps {
                bat 'echo "Bootloading..."'
            }
        }
        stage('Test') {
            steps {
                bat 'pytest'
            }
        }
    }
}