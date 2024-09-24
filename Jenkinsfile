pipeline {
    agent any

    tools {
        jdk 'JAVA_HOME'     // This should match the JDK name in Jenkins (e.g., JAVA_HOME)
        maven 'M2_HOME'     // This should match the Maven name in Jenkins (e.g., M2_HOME)
    }

    stages {
        stage('GIT') {
            steps {
                git branch: 'main',
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
