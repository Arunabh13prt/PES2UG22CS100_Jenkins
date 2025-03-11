pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'g++ -o hello_exec main/hello.cpp'
            }
        }
        stage('Test') {
            steps {
                sh 'invalid command and raises error hopefully'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying Application...'
            }
        }
    }
    post {
        failure {
            echo 'Pipeline Failed!'
        }
    }
}
