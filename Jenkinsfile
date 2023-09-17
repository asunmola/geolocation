pipeline{
    agent any
    tools{
        maven 'M2_HOME'
    }
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
        stage('upload artifact'){
            steps{
            nexusArtifactUploader artifacts: 
            [[artifactId: 'bioMedical', classifier: '', file: 'target/bioMedical-0.0.4-SNAPSHOT.jar', type: 'jar']], 
            credentialsId: 'Nexus-ID', 
            groupId: 'qa', 
            nexusUrl: '198.58.119.40:8081', 
            nexusVersion: 'nexus3', protocol: 'http', 
            repository: 'ayodele-repo', 
            version: '004'
            }
        }    
    }
   
}