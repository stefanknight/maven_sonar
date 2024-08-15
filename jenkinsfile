     pipeline {
        agent none
        stages {
         
          stage("build & sonarqube") {
            agent any
            steps {
              withSonarQubeEnv('New_Scanner') {
                sh 'mvn clean package sonar:sonar'
              }
            }
          }
        }
      }
