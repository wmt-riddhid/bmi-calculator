pipeline {
    agent any

    tools {nodejs "node"}
    // environment {
    //         CI = 'true'
    //     }
    stages {

        stage('check') {
            steps {
                sh 'npm config ls'
            }
        }

        stage('Build') {
            steps {
                sh 'npm install'
            }
        }
        stage('Test') 
            //steps {
                //sh './jenkins/scripts/test.sh'
        stage('Deliver') {
            steps {
                //sh './jenkins/scripts/deliver.sh'
                input message: 'Finished using the web site? (Click "Proceed" to continue)'
                //sh './jenkins/scripts/kill.sh'
            }
        }
    }
}