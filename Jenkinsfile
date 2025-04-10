pipeline {
    agent none
    stages {
        stage('Example Build') {
            steps {
                echo 'Hello World'
            }
        }
        stage('Example Test') {
            step {
                echo 'Hello Test'
            }
        }
        stage('Example Deploy') {
            steps {
                echo 'Deploying'
            }
        }
    }
     post { 
        always { 
            echo 'I will always say Hello again!'
        }
        success { 
            echo 'I will say Hello when pipeline is success'
        }
        failure { 
            echo 'This run when Pipeline is failed, used generally to send more alerts'
        }
    }
}