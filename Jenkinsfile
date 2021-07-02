pipeline {
    agent any
    environment {
        PATH="/usr/share/maven/bin/:$PATH"
    }

    stages {
        stage('fetching') {
            steps {
                //echo 'Hello World'
                git 'https://github.com/SanthoshKumar-GitHub/hello-world-war.git'
            }
        }
        stage('packaging') {
            steps {
                //echo 'Hello World'
                sh "mvn clean package"
            }
        }
    }
}
