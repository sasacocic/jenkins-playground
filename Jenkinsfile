
/* Requires the Docker Pipeline plugin */

// seems like it will run something in a docker container. still no idea what most of this stuff means.
pipeline {
    agent { docker { image 'golang:1.24.5-alpine3.22' } }
    stages {
        stage('build') {
            steps {
                sh 'go version'
            }
        }
    }
}



