pipeline {
    agent any
    stages {
        stage('Example') {
            steps {
                echo 'Hello World'
            }
        }
    }
    post { 
        always { 
            echo 'I will always say Hello again!'
        }
        success {
            echo  'I will say hello when it is success'
        }
        failure {
            echo  'I will not say hello when it is failure'
        }
    }
}