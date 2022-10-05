pipeline {
    agent any

    stages {
        stage('SCA') {
            steps {
                echo 'Code Quality..'
                sh 'mvn sonar:sonar'
            }
        }
        stage('Clean') {
            steps {
                echo 'Building..'
                sh 'mvn clean'
            }
        }
        stage('Validate') {
            steps {
                echo 'Testing..'
                sh 'mvn validate'
            }
        }
        stage('Compile') {
            steps {
                echo 'Deploying....'
                sh 'mvn compile'
            }
        }
        stage('Test') {
            steps {
                echo 'Deploying....'
                sh 'mvn test'
            }
        }
        stage('Package') {
            steps {
                echo 'Deploying....'
                sh 'mvn package'
            }
        }
         stage('Verify') {
            steps {
                echo 'Deploying....'
                sh 'mvn verify'
            }
        }
         stage('Install') {
            steps {
                echo 'Deploying....'
                sh 'mvn install'
            }
        }
    }
}
