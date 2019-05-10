pipeline {
    agent {label 'node1'}
    stages {
        stage('Env Print') {
            steps {
                sh 'env'
            }
        }
    }
    post {
        always {
            deleteDir()
        }
    }
}
