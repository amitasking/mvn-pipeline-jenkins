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
    }
}
