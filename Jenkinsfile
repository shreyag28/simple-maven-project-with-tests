pipeline {
    agent {
    label 'master'
    }

    tools {
        maven "Maven"
    }

    stages {
        stage('Build') {
            steps {
               
              //  git 'https://github.com/shreyag28/SonarQube-Report.git'

                
               // bat "mvn -Dmaven.test.failure.ignore=true clean package"
                
                echo "hello mail demo"

                
            }

            post {
                
                always {
                    emailext body: 'Summary of the project ', subject: 'Jenkins build', to: 'shreyag@cybage.com'
                   
                }
            }
        }
    }
}
