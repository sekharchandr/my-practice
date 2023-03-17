pipeline {
    agent any
    
    tools{
        maven 'maven-3.6.3'
    }

    stages {
        stage('code checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/sekharchandr/my-centralrepository.git'
            }
        }
        
        stage('mvn build'){
            steps{
                sh 'mvn -v'
                sh 'mvn clean package'
            }
        }
    }
}
