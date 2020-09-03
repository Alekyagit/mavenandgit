
node {
   // This is to demo github action	
	stage ('SCM Checkout'){
	git 'https://github.com/Alekyagit/mavenandgit.git'
}
 stage('Compile-Package'){
	   // get maven hone path
	def mvn = tool name: 'maven', type: 'maven'
	   sh "${mvn}/bin/mvn package"
   }
}
