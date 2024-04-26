#!/usr/bin/env groovy

pipeline {
    agent none
    stages {
         stage('test') {
            steps {
                script {
                    echo "Testing the application..."
                }
            }
        }

        stage('build') {
            when{
                BRANCH_NAME == 'master'
            }
            steps {
                script {
                    echo "Building the application..."
                }
            }
        }
       
        stage('deploy') {
            when{
                BRANCH_NAME == 'master'
            }
            steps {
                script {
                    echo "Deploying the application..."
                }
            }
        }
    }
}
