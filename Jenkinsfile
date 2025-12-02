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
                powershell """
                    \$phpPath = "\${env.WORKSPACE}\\php\\php.exe"
                    & \$phpPath "\${env.WORKSPACE}\\index.php"
                """
            }
        }
    }
}
