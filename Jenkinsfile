pipeline {
    agent any

    stages {
        stage('Code-Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/sekharchandr/my-centralrepository.git'
            }
      
       }
       
       stage('mvn build'){
           steps {
               sh 'mvn clean package'
           }
       }
    }
}
