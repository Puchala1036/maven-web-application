pipeline {
    agent any
    
    tools {
        maven 'maven'
    }
    
    triggers {
        githubPush()
    }
    

    stages {
        stage('git clone') {
            steps {
                 git 'https://github.com/Puchala1036/maven-web-application.git'
            }
        }
       stage('maven') {
            steps {
                 sh 'mvn clean package'
            }
        }
        
    }
}
