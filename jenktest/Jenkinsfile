def S3_BUCKET = 'jenktest-nex-ui-dev'
pipeline {
    agent any
    stages {
        stage('NPM Install') {
            steps {
                sh 'cd jenktest'
                    sh 'pwd'
                    sh 'npm install'
            }
        }
        stage('Build') {
            steps {
                sh 'ng build --prod'
            }
        }
    }
}