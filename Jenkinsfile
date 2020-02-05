node {
     def app
 
     stage('Clone repository') {
         /* Let's make sure we have the repository cloned to our workspace */
 
         checkout scm
     }
     stage('Docker Build') {
       agent any
       steps {
         sh 'docker-compose up --build -d'
       }
	 stage('Email Notification'){
	    mail bcc: '', body: 'Report for Jenkins Pipeline jobs ', cc: '', from: '', replyTo: '', subject: 'Jenkins Jobs', to: 'saiprasad169@gmail.com'
	    
	 }
     }
    }
