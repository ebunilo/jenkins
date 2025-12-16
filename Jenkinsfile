Jenkinsfile (Declarative Pipeline) --- IGNORE ---
/* Requires the Docker Pipeline plugin */
pipeline {
    agent { docker { image 'python:3.14.2-alpine3.23' } }
    stages {
        stage('build') {
            steps {
                sh 'python --version'
                sh 'echo "Hello World"'
                sh '''
                    echo "Multiline shell steps works too"
                    ls -lah
                '''
            }
        }
    }
}