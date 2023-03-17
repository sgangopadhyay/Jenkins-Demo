pipeline{
    agent any
    stages{
        stage('Checkout'){
            steps{
                checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/sgangopadhyay/Jenkins-Demo.git']])
            }
        }
        stage('Build'){
            steps{
                git branch: 'main', url: 'https://github.com/sgangopadhyay/Jenkins-Demo.git'
                bat 'python at_11.py'
            }
        }
    }
}
