node {

    stage('rebuildApp') {
      environment {
        GOPATH = "frogs"
      }
    
      git(
        url: 'https://github.com/craigwongva/smallgo.git',
        branch: "master"
      )
      
      sh """
pwd # /var/lib/jenkins/workspace/src/smallgo
echo $GOPATH
go install ./pkg/smallgok
"""
 }
}
