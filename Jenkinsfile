pipeline {
    agent any 
    tools {
         maven 'maven'
         jdk 'JAVA'
    }
    stages {
        /*stage('Stage-0 : Sonar Code Analysis') { 
            steps {
                sh 'mvn clean verify sonar:sonar'
            }
        }
        */
        stage('Stage-1 : Clean') { 
            steps {
                sh 'mvn clean'
            }
        }
        stage('Stage-2 : Validate') { 
            steps {
                sh 'mvn validate'
            }
        }
        stage('Stage-3 : Compile') { 
            steps {
                sh 'mvn compile'
            }
        }
        stage('Stage-4 : Test') { 
            steps {
                sh 'mvn test'
            }
        }
        stage('Stage-5 : Verify') { 
            steps {
                sh 'mvn verify'
            }
        }
        stage('Stage-6 : Package') { 
            steps {
                sh 'mvn package'
            }
        }
        stage('Stage-7 : Install') { 
            steps {
                sh 'mvn install'
            }
        }
       stage('Stage-8 : Deploy') { 
            steps {
                sh 'mvn deploy'
            }
        }
    }
}
