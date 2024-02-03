pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=napasornss -Dsonar.organization=Napasornss -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=60c28a098f0b2671cd673aef110c41cac9662882'
			}
        } 
  }
}
