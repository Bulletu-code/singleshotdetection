pipeline{
    agent any
    stages{
        stage("SCM Checkout"){
            steps{
            git 'https://github.com/Bulletu-code/singleshotdetection'
            }
        }
        stage("COMPILE"){
            steps{
                bat 'mvn compile' 
            }
        }
        stage("TEST"){
            steps{
                bat 'mvn verify' 
            }
        }
        stage("INSTALL"){
            steps{
                bat 'mvn install' 
            }
        }
    }
}

