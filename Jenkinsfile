#!/usr/bin/env groovy
properties([
    [$class: 'GithubProjectProperty',
    displayName: '',
    projectUrlStr: 'https://github.com/chvaraprasad/vp1/'],
   pipelineTriggers([
     
    upstream(
      threshold: 'SUCCESS',
      upstreamProjects: 'https://github.com/taskbuilder/vp3/')
    ])
])
pipeline {
    agent any 

    stages {
        stage('Build') { 
            steps { 
                sh 'pwd' 
            }
        }
        stage('Test'){
            steps {
                sh 'java -version'
                
            }
        }
        stage('Deploy') {
            steps {
                sh 'ls'
                sh 'pwd'
            }
        }
    }
}
