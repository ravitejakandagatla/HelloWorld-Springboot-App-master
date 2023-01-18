pipeline {
    agent any
    stages {
        stage('Git Clone'){
            steps{
            git branch: 'main', url: 'https://github.com/ravitejakandagatla/HelloWorld-Springboot-App-master.git'
        }
    }
    stage('Maven Test'){
            steps{
            bat 'mvn test'
        }
    }
    stage('Maven Build'){
            steps{
            bat 'mvn package'
        }
    }
    stage('Maven Deploy'){
            steps{
            echo "Deployinh the war file to server"
        }
    }
}
}
