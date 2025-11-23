pipeline {
    agent { label 'dev' }

    tools {
        maven 'mymaven'
    }

    stages {
        stage ('code') {
            steps {
                git url: 'https://github.com/sivam792/one.git'
            }
        }
        stage ('build') {
            steps {
               sh 'mvn clean package'
            }
        }
        stage ('deploy') {
            steps {
               deploy adapters: [tomcat9(alternativeDeploymentContext: '', credentialsId: 'tom', path: '', url: 'http://3.15.240.72:8080/')], contextPath: 'cat', war: 'target/*.war' 
            }
        }
    }
}
