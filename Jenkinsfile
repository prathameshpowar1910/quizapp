pipeline {
    agent any
    tools{
        maven 'maven_399'
    }
    stages{
        stage('Build Maven'){
            steps{
                checkout scmGit(branches: [[name: '*/master']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/prathameshpowar1910/quizapp']])
                mvn -B -DskipTests clean package
            }
        }
        
    }
}
