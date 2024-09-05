pipeline {
    agent { label 'slave1' }
    tools {
      //maven 'maven3'
      jdk 'jdk17'
    }
    
    stages {
        // stage('Git Checkout') {
        //     steps {
        //         git branch: 'main', url: 'https://github.com/vijkes/FullStack-Blogging-App.git'
        //     }
        // }
        stage('Compile') {
            steps {
                sh 'mvn compile'
            }
        }
        stage('Test') {
            steps {
                sh 'mvn test'
            }
        }
        stage('Package') {
            steps {
                sh 'mvn package'
            }
        }

    }
}
