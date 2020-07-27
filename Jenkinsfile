@Library('utils') _
  
if (env.CHANGE_ID) {
       def APPLICATION_NAME = "${env.JOB_NAME}".split('/').first()
       deploy("${APPLICATION_NAME}","${CHANGE_ID}")
}else{
       stage('ALERT'){ echo 'Please build app from Pull Requests' }
}
