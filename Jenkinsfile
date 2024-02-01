pipeline {
    agent{
        node {
            label 'AGENT-1'
        }
    }
    // Build
    stages {
        stage('Build') {
            steps {
                echo 'Building..'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
    // post build
    post {
        always {
            echo 'I will always say hello'
        }
        failure {
            echo 'This run when pipeline is failed, used generally to send some alerts'
        }
        success {
            echo 'I will say Hello when pipeline is seccess'
        }
    }
}