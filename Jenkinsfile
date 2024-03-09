pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'g++ temp.cpp -o temp'
                 build job: 'PES1UG21CS290-1', wait: false
                 echo 'Build by CS290 successful'
            }
        }

        stage('Test') {
            steps {
                sh 'cat temp.cpp'
                echo 'Test by CS290 successful'
            }
        }

        stage('Deploy') {
            steps {
               
                 ech 'Deploy by CS290 successful'
            }
        }
    }

    post {
        failure {
            
                echo 'Pipeline Failed'
          
        }
    }
}
