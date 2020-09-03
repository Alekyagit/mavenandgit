
node {
   // This is to demo github action	
   stage ('SCM checkout')
	git 'https://github.com/Alekyagit/mavenandgit.git'
}
 stage('Mvn Package'){
	   // Build using maven 
	def mvn = tool name: 'maven', type: 'maven'
	   sh "${mvn}/bin/mvn clean package deploy"
   }
   
   stage('Email Notification'){
		mail bcc: '', body: """Hi Team, You build successfully deployed

Thanks,
DevOps Team""", cc: '', from: '', replyTo: '', subject: "${env.JOB_NAME} Success", to: 'alekyajune19@gmail.com'
   
   }

