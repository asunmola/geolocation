pipeline{
    agent any
    stages {
        stage('maven clean'){
            steps{
            sh 'mvn clean'
            }
        }
        stage('install'){
            steps{
            sh 'mvn install'
            }
        }
        stage('package'){
            steps{
            sh 'mvn package'
            }
        }
        stage('liverpool'){
            steps{
            sh 'echo liverpool'
            }
        }
        stage('clean artifact'){
            steps{
            sh 'echo hi'
            }
        }
    }
   
}