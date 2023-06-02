def S3_BUCKET = 'jenktest-nex-ui-dev'
pipeline {
    agent any
    stages {
        stage('NPM Install') {
            steps {
                script {
                    notifyBitbucket(buildStatus: 'INPROGRESS')
                }
                sh 'cd jenktest'
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