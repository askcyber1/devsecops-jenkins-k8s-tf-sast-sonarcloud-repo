pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=jenkinakin -Dsonar.organization=Jenkinakinbuggy -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=26c4827cef24ed417e59dedcaa23b4c4b31c17cd'
			}
        } 
  }
}
