pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=roroweb123 -Dsonar.organization=roroweb123 -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=6f78b80e294cfd93ef205258661f912a81befb8d'
			}
        } 
  }
}
