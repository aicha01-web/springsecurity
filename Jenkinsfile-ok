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
    }
}
