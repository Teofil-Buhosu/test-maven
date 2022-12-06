pipeline {
    tools {
        maven 'Maven3'
    }
    agent any 
    stages {
        stage ('Initialize') {
            steps { 
                sh ''' echo "PATH = ${PATH}" echo "M2_HOME = ${M2_HOME}" ''' 
            }
        }
        stage('maven install') {
            steps {
                sh 'mvn clean install'
            }
        }
    }
}
