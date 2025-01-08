pipeline {
    agent any
    tools{
        maven "mvn3.9.8"
    }

    stages {
        // stage('Git Checkout') {
        //     steps {
        //         git branch: 'main', url: 'https://github.com/Learning-DevSecOps/jenkins-hello-world.git'
        //     }
        // }
        stage('Build') {
            steps {
                sh "mvn clean package -DskipTests=true"
            }
        }
        stage('test') {
            steps {
                sh "mvn test"
            }
        }
    }
}
