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
                // sh "mkdir -p /usr/local/var/www/node-app"
                sh "rm -rf /usr/local/var/www/node-app"
                sh "cp -R /Users/VAIBHAV/AppData/Local/Jenkins/.jenkins/workspace/weatherapp /usr/local/var/www/node-app"
            }
        }
    }
}