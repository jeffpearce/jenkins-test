node('node') {
   stage('Stage  1') {
    print 'upstream job stage 1';

    def downstreamTasks = [:];

    downstreamTasks["downstream"] = {
       build job: 'Jeff Pearce/jenkins-test-downstream/master',
       parameters: []
    };

    parallel downstreamTasks       
   }
}
