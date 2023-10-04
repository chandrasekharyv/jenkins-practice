pipeline {
    agent {
        node {
           label 'Agent'
        }
        
    }
    options {
        ansiColor('xterm')
    }

    stages {
        stage('Build') {
            steps {
                echo 'Building....'
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
                // error 'job is failure'
            }
        }
    }

    post { 
        always { 
            echo 'I will always run job is success or not !'
        }
        success {
            echo 'i will run when the job is success'
        }
        failure {
            echo 'i will run when job is failure'
        }
    }
}