pipeline{
	agent any
	stages{
		stage('build')
		{
			steps{
				sh "whoami"
				sh "mvn clean package"
				sh "docker build . -t tomcatwebapp:${env.BUILD_ID}"
			}
		}
	}
}