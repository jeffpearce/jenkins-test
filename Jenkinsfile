node('node') {
   stage('Stage  1') {
     print 'upstream job stage 1'
       build job: './Jenkinsfile.downstream',
         parameters: []
   }
}
