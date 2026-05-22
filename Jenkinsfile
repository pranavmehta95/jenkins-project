pipeline {
    agent any

    stages {

        stage('Build Docker Image') {
            steps {
                script {
                    docker.build("my-python-app")
                }
            }
        }

        stage('Run Container') {
            steps {
                sh 'docker run --rm my-python-app'
            }
        }
    }
}
