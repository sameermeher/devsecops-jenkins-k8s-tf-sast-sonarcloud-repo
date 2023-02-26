pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asgbuggywebapp-sameermeher -Dsonar.organization=asgbuggywebapp-sameermeher -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=66a9d34ae8e92e419b9fa552e23e9d4c1acc590d'
			}
        } 
  }
}
