pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                git 'https://github.com/yourusername/prime-checker.git'
            }
        }

        stage('Build') {
            steps {
                bat 'mvn clean package'
            }
        }

        stage('Run') {
            steps {
                bat 'java -cp target/prime-checker-1.0-SNAPSHOT.jar com.example.App'
            }
        }
    }
}
