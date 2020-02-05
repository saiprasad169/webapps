node {
     def app 
	 stage('Email Notification'){
	    mail bcc: '', body: '''Jenkins Success
            Thanks''', cc: '', from: '', replyTo: '', subject: 'TEST', to: 'saiprasad169@gmail.com' 
       }
         stage('Deploy on kubernetes') {
            sh "kubectl apply -f kube-dev.yml"
         }
     }
