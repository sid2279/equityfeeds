pipeline {
    agent any
    tools {
        maven 'maven_3_6_3'
    } 
    stages {
        stage ('Compile Stage') {

            steps {
                bat "mvn clean install compile"
            }
        }

        stage ('Testing Stage') {

            steps {
                bat "mvn test"
            }
        }


        stage ('Deployment Stage') {
            steps {
                bat "mvn deploy"
            }
        }
    }
}
