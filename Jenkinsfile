pipeline {
  agent any
  tools { 
        maven 'Apache-MAVEN'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=Napasornss -Dsonar.organization=Napasornss -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=5d9007dd536e001aec886ab02330040867fa573e'
			}
        } 
  }
}
