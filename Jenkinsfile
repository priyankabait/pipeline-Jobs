pipeline {
    agent any

    stages {
        stage('Use Jenkins Java 17') {
            tools {
                jdk 'JAVA-17'
            }

            steps {
                echo 'Using Jenkins-managed Java'
                bat 'java -version'
                bat 'echo JAVA_HOME=%JAVA_HOME%'
            }
        }

        stage('Use System Java 21') {
            steps {
                echo 'Using system-installed Java 21.0.12'
                bat '"C:\\Program Files\\Java\\jdk-21.0.12\\bin\\java.exe" -version'
            }
        }

        stage('Use Jenkins Java Again') {
            tools {
                jdk 'JAVA-17'
            }

            steps {
                bat 'java -version'
            }
        }
    }
}



