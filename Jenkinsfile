pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git url: 'https://github.com/LiftyPavita/test.git', branch: 'main'
            }
        }

        stage('Run PHP') {
            steps {
                powershell """
                    php "${env.WORKSPACE}/index.php"
                """
            }
        }
    }
}
