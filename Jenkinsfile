pipeline {
    agent any
    stages {
        stage("clean up"){
            steps {
                deleteDir()
            }
        }
        stage("Clone Repo") {
            steps {
                sh "git clone https://github.com/DalimAli/Jenkins.git"
            }
        }
        stage("Build"){
            steps{
                dir("Jenkins"){
                    sh "mvn clean install"
                }
            }
        }
    }
}