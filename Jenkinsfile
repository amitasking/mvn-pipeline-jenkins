pipeline {
    agent any

 

    stages {
        stage('build') {
            steps {
                sh 'mvn -version'
            }
            steps {
                sh 'mvn clean package'
            }
        }
        
        stage('deploy') {
            steps {
                sh 'deploy adapters: [tomcat9(credentialsId: '6e3ed345-0389-4d97-9d95-ef3568aeb444', path: '', url: 'http://13.127.147.9:8080/')], contextPath: 'MyWebApp', war: 'MyWebApp.war''
            }
        }
    }
}
