pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=newjenkinsakin -Dsonar.organization=newjenkinsakin -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=656b8426fb4e7f960802824fc2f2b7bf181eb6fa'
			}
        } 
  }
}
