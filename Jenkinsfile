pipeline {
    agent any

    stages {
        stage('Cloning Git Repository') {
            steps {
                git branch: 'main', url: 'https://github.com/rejaine-sm/jk-public-gh.git'
                }
        }
        
        stage('Build Image') {
            steps {
                sh 'docker build -t webapp:${BUILD_NUMBER} .'
                }
        }                      
    }
}
