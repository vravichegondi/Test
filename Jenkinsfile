pipeline {
    agent any
    stages {
        stage('Build Application') {
            steps {
                bat 'mwn clean install'
            }
        }
        stage('Deploy Application To Mulesoft Cloudhub') {
            steps {
                bat 'mwn package deploy -DmuleDeploy'
            }
        }

        
        /* stage('Perform Regression Testing') {
            steps {
                bat 'c:\\users\\Jitendra\\AppData\\Roaming\npm\\newman run F:\\newman\\worldtimezone.postman_collection.json --disable-unicode'
            }
        } */
    }
}
