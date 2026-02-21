pipeline {
  agent any
  tools { 
        maven 'Maven_3_8_4'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=mmbuggywebapp -Dsonar.organization=mmbuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=363744f02b4367747d67f3029802dd91b5f4c343'
			}
        } 
  }
}
