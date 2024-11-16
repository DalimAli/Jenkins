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
                sh "git clone https://github.com/DalimAli/Simple-Jenkins-App.git"
            }
        }
        stage("Build"){
            steps{
                dir("Simple-Jenkins-App"){
                    sh "mvn clean install"
                }
            }
        }
        stage("Test"){
            steps{
                dir("Simple-Jenkins-App") {
                    sh "mvn test"
                }
            }
        }
    }
}
