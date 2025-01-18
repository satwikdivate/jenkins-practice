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
                    def prohjectName=params.PROJECT_NAME?:PROJECT_NAME
                    bat 'echo "Your Project Name: ${projectName}"'
                    bat 'echo "Your SetName: ${SET_NAME}"'
               }
            }
        }
    }
}
