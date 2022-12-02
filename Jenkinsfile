pipeline {
    agent any
    stages {
        stage('SCM') {
            steps {
                echo 'Code Quality..'
                sh 'mvn sonar:sonar'
            }
        }
        stage('Clean') {
            steps {
                echo 'Clean..'
                sh 'mvn clean'
            }
        }
        stage('Validate') {
            steps {
                echo 'Validate..'
                sh 'mvn validate'
            }
        }
        stage('Compile') {
            steps {
                echo 'Compile....'
                sh 'mvn compile'
            }
        }
        stage('Test') {
            steps {
                echo 'Test....'
                sh 'mvn test'
            }
        }
        stage('Package') {
            steps {
                echo 'Package....'
                sh 'mvn package'
            }
        }
         stage('Verify') {
            steps {
                echo 'Verify....'
                sh 'mvn verify'
            }
        }
         stage('Install') {
            steps {
                echo 'Install....'
                sh 'mvn install'
            }
        }
        //  stage('Deploy') {
        //     steps {
        //         echo 'Deploy....'
        //         sh 'mvn deploy'
        //     }
        // }
        //  stage('Deliver and Deployment') {
        //     steps {
        //         echo 'Deliver and Deployment....'
        //         sh ''
        //     }
        // }
    }
}
