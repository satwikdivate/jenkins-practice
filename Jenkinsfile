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
                // Replace 'Shri Ganesh' with a valid shell command or script
                bat 'echo "Shri Ganesh"'

                bat 'echo "Your ProjectName: ${PROJECT_NAME}"'
                bat 'echo "Your SetName: ${SET_NAME}'
            }
        }
    }
}
