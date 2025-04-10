pipeline {
    agent {
        label 'Agent-1'
    }
    options {
        timeout(time: 10, unit: 'SECONDS')
        disableConcurrentBuilds()
        // retry()
    parameters {
        string(name: 'Greeting', defaultValue: 'Hello', description: 'How should I greet the world?')
    }
    }
    stages {
        stage('Example') {
            steps {
                echo 'Hello World'
                // error 'pipeline failed'
                // sleep(10)
        
        stage('Example') {
            steps {
                echo "${params.Greeting} World!"
            }
        }    
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