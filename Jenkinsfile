#!/usr/bin/env groovy
pipeline{
    agent any
    stages{
        stage("cleaning the work space"){
            steps{
                sh 'rm -rf *'
            }
        }      
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