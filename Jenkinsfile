pipeline{
    agent any
    stages{
        stage('clone repository') {
            steps{
                git branch: 'main', url: 'https://github.com/Chennakeshava22/Spring-boot-application.git' 

            }
        }
        stage('mvn test'){
            step{
                sh 'mvn test'

            }
        }
        stage('build'){
            step{
                sh 'mvn install -DskipTests'
            }
        }
    }
}
