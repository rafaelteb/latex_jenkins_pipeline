pipeline {
    agent none
    stages {
        stage('Build') {
            agent {
                docker {
                   image 'leplusorg/latex'
                }   
            }
            steps {
                sh 'ls -la'
                sh 'latexmk -pdf latex/sample.tex'
            }
        }
    }
}
