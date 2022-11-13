pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=skyglassbuggy -Dsonar.organization=skyglassbuggy -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=e182285560cfbd5446a40330354ebca6477db5e0'
			}
        } 
  }
}
