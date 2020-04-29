pipeline {
     agent any
        stage('Upload to AWS') {
              steps {
                  withAWS(region:'us-west-2',credentials:'aws-static') {
                      s3Upload(file:'index.html', bucket:'jstaticbucket', path:'/')
                  }
              }
         }
}