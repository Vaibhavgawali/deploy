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
                sh "rm -rf /usr/local/var/www/node-app"
                sh "cp -R /users/aakash/.jenkins/workspace/WeatherApp /usr/local/var/www/node-app"
            }
        }
    }
}