pipeline {
    agent any

    stages { 

        stage('Build'){
                steps{
                    bat 'mvn clean package'
                    bat "docker build . -t eng:${env.BUILD_ID}"
                }
            }

    }

}
