pipeline {

    agent any

    triggers {
        githubPush()
    }

    stages {

        stage('GIT') {
            steps {
                git branch: 'master',
                url: 'https://github.com/macherkiJawher/jawher-macherki-4twin8.git'
            }
        }

        stage ('Compile Stage') {
            steps {
                sh 'mvn clean compile'
            }
        }
    }
}
