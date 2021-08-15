#!/usr/bin/env groovy
pipeline{
    agent any
    stages{   
        stage("testing maven"){
            steps{
                dir("mvn"){
                sh 'mvn test'
                }
            }
        }
        stage("maven package"){
            steps{
                dir("mvn"){
                sh 'mvn package'
                }
            }
        }
    }
}