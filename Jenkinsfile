pipeline {
    agent any
    stages {
        stage('---clean---') {
            steps {
                sh "clean install package"
            }
        }
        stage('--test--') {
            steps {
                sh "mvn test"
            }
        }
        stage('--package--') {
            steps {
                sh "mvn package"
            }
        }
    }
}
