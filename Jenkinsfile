pipeline {
    agent any
    stages {
        stage(‘Build’) {
            steps {
                 sh "/usr/local/Cellar/maven/3.8.7/bin/mvn clean package"
            }
        }
        stage(‘Test’) {
            steps {
                 sh "/usr/local/Cellar/maven/3.8.7/bin/mvn test"
            }
        }
        stage('Deploy') {
            steps {
                sh '/Applications/Docker.app/Contents/Resources/bin/docker-compose-v1/docker-compose up -d --build'
            }
        }
    }
}
