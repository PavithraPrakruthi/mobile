pipeline {
agent any

stages {
         
           stage('Cloning our Git') {

            steps {

                git branch: 'master', url: 'https://github.com/kliakos/sparkjava-war-example.git'
                sh 'ls'

            }

             }
		
		   stage('build') {
		   
		   steps {
		     sh "mvn install"
		   }
		   }
		   
		   stage('deployment') {
		   
		   steps {
		   sh "ansible --version"
		   }
		   }


}



}
