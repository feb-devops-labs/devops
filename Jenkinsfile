#!groovy

def appname='devops'
def env='production'
pipeline{
agent any
   stages {
        stage('Clean Workspace') {
            steps {
                deleteDir()
                echo 'Cleeanup done'
            }
        }
		stage('cloning'){
		steps{
			checkout scm
			}
		}
		stage('build'){
		steps{
			sh'mvn clean install'
			}
		}
	}	
}
