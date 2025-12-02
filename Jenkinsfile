pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/LiftyPavita/test.git'
            }
        }

        stage('Run PHP') {
            steps {
                powershell 'php index.php'
            }
        }
    }
}
