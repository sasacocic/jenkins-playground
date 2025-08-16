
/* Requires the Docker Pipeline plugin */

// seems like it will run something in a docker container. still no idea what most of this stuff means.
@Library("jenkins-pipeline-library@main") _
pipeline {
    // agent: tells jenkins where and how to execute the pipeline, or subset there of - required for all pipelines
    agent { docker { image 'golang:1.24.5-alpine3.22' } }
    stages {
        stage('build & test') {
            steps {
                println "yes"
                foo()
                sh 'go version'
                sh 'go test ./cmd/...'
            }
        }
    }
}



