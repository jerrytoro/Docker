pipeline {
    agent {label 'debian_server'}

    stages {
        stage('cloning') {
            steps {
                git branch: 'main', url: 'https://github.com/jerrytoro/Docker.git'
            }
        }
        stage ('build') {
            steps {
                sh "docker compose ps"
            }
        }
    }
}
