pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=Napasornss -Dsonar.organization=Napasornss -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=005af9f632c37932b9c47ce90d87cf2f13fbd22d'
			}
        } 
  }
}
