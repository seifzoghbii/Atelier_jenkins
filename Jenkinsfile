pipeline {
    agent any

    tools {
        jdk 'JAVA_HOME'     // Use the correct JDK name from Jenkins
        maven 'M2_HOME'     // Use the correct Maven name from Jenkins
    }

    stages {
        stage('Checkout') {
            steps {
                git branch: 'master',  // Explicitly use 'master' branch
                url: 'https://github.com/seifzoghbii/Atelier_jenkins.git'
            }
        }

        stage('Compile Stage') {
            steps {
                sh 'mvn clean compile'
            }
        }
    }
}
