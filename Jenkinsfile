pipeline {
    agent any
    stages {
        stage('Checkout Code') {
            steps {
                git branch: 'main', url: 'https://github.com/tamiltamil08263-web/jenkins-s3-demo.git'
            }
        }
        stage('Deploy to S3') {
            steps {
                sh 'aws s3 cp index.html s3://jenkins-demo-tamil/ --acl public-read'
            }
        }
    }
}
