pipeline{
	agent any
	stages{
		stage('build')
		{
			steps{
				sh "mvn clean package"
				sh "docker build . -p  -t tomcatwebapp:${env.BUILD_ID}"
			}
		}
	}
}