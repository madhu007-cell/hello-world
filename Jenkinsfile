pipeline {
    agent any
    stages{
        stage ( 'Compile Stage') {
            
            steps {
                withMaven(maven : 'apache-maven-3.6.3') {
                    sh 'mvn clean complile'
                }
             }
        }
        stage   ('Testing Stage') {
            steps {
                withMaven(maven : 'apache-maven-3.6.3') {
                    sh 'mvn test'
                }
            }
        } 
        stage ('Install Stage') {
            steps {
                withMaven(maven : 'apache-maven-3.6.3') {
                    sh 'mvn install'
                }
            }
        }
    }
}   

