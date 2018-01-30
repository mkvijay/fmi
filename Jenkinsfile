#!groovy
@Library('my-shared-library') _
pipeline {
    agent none 
    stages {
        stage('Example Build') { 
            steps {
                echo 'Hello, Maven'
            }
        }
        stage('Example Test') { 
            steps {
                echo 'Hello, JDK'
            }
        }
    }
}

