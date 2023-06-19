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
                sh "rm -rf /nginx/html/node-app"
                sh "cp -R /Users/VAIBHAV/AppData/Local/Jenkins/.jenkins/workspace/weatherapp /nginx/html/node-app"
            }
        }
    }
}