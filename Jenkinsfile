#!groovy

node {
    checkout scm
    stage('Build') {
        withCredentials([usernamePassword(credentialsId: 'credentials_dont_exist', passwordVariable: 'MY_PASSWORD', usernameVariable: 'MY_USERNAME')]) {

            sh "./mvnw clean install"
        }
    }
}