pipeline {
  agent any
  stages {
    stage('SCM') {
      steps {
        parallel(
          "SCM": {
            git(url: 'https://github.com/vairamuthu-shanmugaraj/job-dsl-plugin.git', branch: 'master')
            
          },
          "Batch": {
            bat 'dir'
            
          }
        )
      }
    }
  }
}