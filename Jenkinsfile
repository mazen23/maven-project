pipeline{
	agent any
	stages{
		stage('build')
		{
			steps{
				bat "whoami"
				bat "mvn clean package"
				bat "docker build . -t tomcatwebapp:${env.BUILD_ID}"
			}
		}
	}
}