pipeline {
    agent {
        label 'Agent-1'
    }
    options {
        timeout(time: 10, unit: 'SECONDS')
        disableConcurrentBuilds()
    }
    stages {
        stage('Example') {
            steps {
                echo 'Hello World'
                sleep(10)
            
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
            echo  'I will say hello when it is failure'
        }
    }
}