pipeline {                                  // 1 // Start of pipeline
    agent any                               // Runs on any available agent

    environment {                           // 2 // Environment variables
        PATH = "/opt/maven/bin:$PATH"       // Add Maven to system PATH
    }

    stages {                                // 3 // Stages block
        stage('build') {                    // 5 // Build using Maven
            steps {
                sh 'mvn clean install'
            }
        }
    }
}
