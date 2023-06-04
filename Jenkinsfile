pipeline {
	agent any
	stages {
		stage('Checkout') {
			steps {
				checkout scm
			}} 
			stage ('Build') {
				steps {
					sh '/home/ubuntu/Documents/DevOps_Tools/apache-maven-3.9.1/bin/mvn install'
				}} 
				stage('Deployment') {
				steps {
				sh 'cp target/flipkart.war /home/ubuntu/Documents/DevOps_Tools/apache-tomcat-9.0.73/webapps'
				}
}}}
