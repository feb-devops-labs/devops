pipeline{
agent {
    lable devops
    }
def appname='devops'
def env='production'
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
