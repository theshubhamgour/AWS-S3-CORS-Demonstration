pipeline {
    agent any

    stages {
        stage('Github Code Pulling') {
            steps {
                // Get some code from a GitHub repository
                git 'https://github.com/theshubhamgour/Corpdata.git' 
            }
        }
        stage('Maven Build and Compile'){
            steps{
                sh 'mvn install'
            }
        }
        stage('Apache Hosting'){
            steps{
                sh 'cp target/ben.war //home/theshubhamgour/Documents/softwares/apache-tomcat-9.0.82/webapps'
            }
        }           

    }
}
