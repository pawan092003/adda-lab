pipeline {
    agent any
    
    tools {
        maven "maven-3.9.9"
        jdk "jdk-21"
    }

    stages {
        stage('check out SCM') {
            steps {
                git 'https://github.com/pawan092003/adda-lab.git'
            }
        }
        
        stage('java compile') {
            steps {
                sh 'javac Main.java'
            }
        }
        
        stage('java run') {
            steps {
                sh 'java Main'
            }
        }
    }
}
