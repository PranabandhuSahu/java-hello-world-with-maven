pipeline {
    agent any
    environment {
        PATH = "/opt/maven/bin:$PATH"
    }
    stages {
       
        stage('Git Clone') {
            
            steps {
                git url: 'https://github.com/PranabandhuSahu/java-hello-world-with-maven.git', branch: 'master'
            }
            
        }
        
        stage('build') {
            steps {
                sh 'mvn clean install'
            }
            
        }
    }
}
