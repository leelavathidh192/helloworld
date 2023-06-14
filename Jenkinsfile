pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Checkout the Git repository
                git branch: 'main', credentialsId: 'GITHUBPERSONAL', url: 'https://github.com/leelavathidh192/helloworld.git'
            }
        }

        stage('Build') {
            steps {
                // Run other build steps or commands
                sh 'git status'
                sh 'git commit -m "Commit message"'
                sh 'git push origin main'
            }
        }
    }
}
