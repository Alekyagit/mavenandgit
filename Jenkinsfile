
node {
   // This is to demo github action	
	stage ('SCM checkout'){
	git 'https://github.com/Alekyagit/mavenandgit.git'
}
 stage('Mvn Package'){
	   // get maven hone path
	def mvn = tool name: 'maven', type: 'maven'
	   sh "${mvn}/bin/mvn clean package deploy"
   }
}
