pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                git 'https://github.com/jonathan934422/Maven-Jenkins-Demo.git'
            }
        }

        stage('Build') {
            steps {
                bat 'mvn clean package'
            }
        }

        stage('Deploy') {
            steps {
                bat 'copy target\\Maven-Jenkins-Demo.war "C:\\Users\\acer\\Downloads\\apache-tomcat-10.1.59-windows-x64\\apache-tomcat-10.1.59\\webapps\\"'
            }
        }
    }
}
