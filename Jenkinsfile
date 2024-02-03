pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=napasornss -Dsonar.organization=Napasornss -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=e6adcd22f3de186badef42336209126126153941'
			}
        } 
  }
}
