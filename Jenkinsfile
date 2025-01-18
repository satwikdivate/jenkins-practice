pipeline {
    agent any

    environment{
        PROJECT_NAME= 'JENKINS_PRACTICE'
        SET_NAME= 'SET1'
    }

    parameters{
        string(name:'PROJECT_NAME',defaultValue:'${PROJECT_NAME}',description:'Enter your project name')
        string(name:'SET_NAME',defaultValue:'${SET_NAME}',description:'Enter your setName')
    }
    stages {
        stage('Test') {
            steps {

                script{

                    // Replace 'Shri Ganesh' with a valid shell command or script
                    bat 'echo "Shri Ganesh"'
                    def projectName=params.PROJECT_NAME?:PROJECT_NAME
                    bat "echo \"Your Project Name: ${projectName}\""
                    bat "echo \"Your SetName: ${SET_NAME}\""
               }
            }
        }
        stage('Testing'){

            parallel{
                stage("Unite Testing"){
                    steps{

                        bat "echo \"Unite testing for ${PROJECT_NAME}\""
                    }
                }
                stage("Functional testing"){
                    steps{
                        bat "echo Running Unit Tests for ${SET_NAME}"
                    }
                }
            }
        }
    }
}
