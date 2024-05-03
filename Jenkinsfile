pipeline {
    agent any
    environment {
        JAVA_HOME = '/opt/maven'
    }
    tools { 
        maven 'Maven_3_6_3'  
    }
    stages {
        stage('CompileandRunSonarAnalysis') {
            steps {	
                sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=devscop00 -Dsonar.organization=devsecop0 -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=3cad1defd8607a9a76b7f818f4d5e4b6d3b5a215'
            }
        } 
    }
}
