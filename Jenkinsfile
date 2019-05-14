pipeline {
    agent {label 'node1'}
    stages {
        stage('Env Print') {
            steps {
                sh 'env > output.out'
                printn "$PATH"
                archiveArtifacts 'output.out'
            }
        }
    }
    post {
        always {
            deleteDir()
        }
    }
}
