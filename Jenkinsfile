pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Run PHP') {
            steps {
                script {
                    powershell 'php index.php'
                }
            }
        }
    }
}
