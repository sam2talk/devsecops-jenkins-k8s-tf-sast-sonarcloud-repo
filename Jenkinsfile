pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=devsecop0 -Dsonar.organization=devsecop0 -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=b598fbbd6aff49f7d5162f900f1da7c9eaaf7154'
			}
        } 
  }
}
