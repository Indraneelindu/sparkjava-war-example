pipeline {
    agent any
    environment {
        PATH = "/opt/maven/maven/bin:$PATH"
    }
    stages {
        stage ('Clone GIT') {
            steps {
                git url : 'https://github.com/Indraneelindu/sparkjava-war-example.git', branch: 'master'
            }
        }
        stage ("build") {
            steps {
                sh 'mvn clean install'
            }
        }
    }
}

