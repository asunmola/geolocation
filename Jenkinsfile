pipeline{
    agent any
    stages {
        stage('maven clean'){
            steps{
            mvn clean
            }
        }
        stage('install'){
            steps{
            mvn install
            }
        }
        stage('package'){
            steps{
            sh '/opt/maven/bin/mvn package'
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