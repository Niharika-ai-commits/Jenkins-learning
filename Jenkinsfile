pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh "echo This is build"
            }
        }
        stage('Test') {
            steps {
                sh "echo This is test"
            }
        }
        stage('Deploy') {
            steps {
                sh "echo This is deploy"
            }
        }
    }
    post{
        always{
            echo "This section runs always"
        }
        sucess{
            echo "This section runs when pipeline is success"
        }
        failure{
            echo "this section runs when pipeline is failed"
        }
    }
}