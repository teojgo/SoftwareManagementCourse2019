pipeline {
    agent {label 'node1'}
    stages {
        stage('Env Print') {
            steps {
                sh 'env'
                println "$PATH"
            }
        }
    }
    post {
        always {
            deleteDir()
        }
    }
}
