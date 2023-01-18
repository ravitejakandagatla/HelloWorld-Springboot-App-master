pipeline {
    agent any
    stages {
        stage('Git Clone'){
            steps{
            git branch: 'main', url: 'https://github.com/ravitejakandagatla/HelloWorld-Springboot-App-master.git'
        }
    }
       stage('Maven Build'){
            steps{
            bat 'mvn package'
            }
       }           
    stage('Create Dockerimage'){
            steps{
            bat 'docker build -t mybuildimage --target build-env  .'
         }
     }
  }
}
