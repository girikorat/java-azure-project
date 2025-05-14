pipeline {
    agent any

    stages {
        stage('git clone') {
            steps {
                git 'https://github.com/girikorat/java-azure-project.git'
            }
        }
        stage('maven package') {
            steps {
                sh 'mvn clean package'
            }
        }
    }
}
