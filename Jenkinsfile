pipeline{
    agent any
    tools {nodejs "NodeJS"}
    stages{
        stage("Install"){
            steps{
                sh "npm install"
            }
        }

        stage("Deploy"){
            steps{
                sh "rm -rf C:/nginx/html/node-app"
                sh "cp -R C:/Users/VAIBHAV/AppData/Local/Jenkins/.jenkins/workspace/weatherapp C:/nginx/html/node-app"
            }
        }
    }
}