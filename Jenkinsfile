pipeline {
    agent any
    tools{
maven 'maven3.6.1'
}

    stages {
        stage('git clone') {
            steps {
               git 'https://github.com/Kumarbgm16/java-azure-project.git'
            }
        }
        stage('maven package') {
            steps {
               sh 'mvn clean package'
            }
        }
    }
}
