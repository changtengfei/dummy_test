pipeline {
    agent {
        label 'windows && a102'
    }
    stages {
        stage('Test') {
            steps {
                bat 'mkdir reports'
                bat 'pytest --junitxml=reports/report.xml'
            }
        }
    }
    post {
        always {
            junit 'reports/*.xml'
        }
    }
}