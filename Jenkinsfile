pipeline {
    agent any

    stages {

        stage('Build') {
            steps {
                bat 'mvn clean package'
            }
        }

        stage('Deploy') {
            steps {
                bat 'copy target\\Maven-Jenkins-Demo.war "C:\\Users\\Admin\\Downloads\\apache-tomcat-10.1.59-windows-x64\\apache-tomcat-10.1.59\\webapps\\"'
            }
        }
    }
}
