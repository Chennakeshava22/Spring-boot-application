pipeline{
    agent any
    stages{
        stage('clone repository') {
            steps{
                git branch: 'main', url: 'https://github.com/Chennakeshava22/Spring-boot-application.git' 

            }
        }
        stage('mvn test'){
            steps{
                sh 'mvn test'

            }
        }
        stage('build'){
            steps{
                sh 'mvn install -DskipTests'
            }
        }
    }
}
