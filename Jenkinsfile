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
        sucess {
            echo  'I will say hello when it is sucess'
        }
        failure {
            echo  'I will not say hello when it is failure'
        }
    }
}