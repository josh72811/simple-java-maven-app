pipeline {
    agent {
        docker {
            image 'maven:3.6.3-ibmjava-8-alpine' 
            args '-u root' 
        }
    }
    stages {
        stage('Build') { 
            steps {
                sh 'mvn -B -DskipTests clean package' 
            }
        }
    }
}
