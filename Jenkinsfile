pipeline {
    agent any
    tools
    {
        maven 'maven3.6.1'
    }
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
        stage('Maven Version') {
            steps {
                sh 'mvn --version'
            }
        }
    }
}
