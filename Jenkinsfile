pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'g++ -o PES2UG20CS238-1 try.cpp'
                cho "Build Successful"
            }
        }
        stage('Test') {
            steps {
                sh './PES2UG20CS238-1'
            }
        }
        stage('Deploy') {
            steps {
                sh './PES2UG20CS238-1'
            }
        }
    }
    post {
        always {
            echo 'Pipeline completed'
        }
        failure {
            echo 'Pipeline failed'
        }
    }
}
