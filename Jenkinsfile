pipeline{
  agent any
  stages{
    stage("Bulid"){
      steps{
          echo 'building the project'
      }
    }
     stage("test"){
       when{
         expression{
           BRANCH_NAME=='master'
         }
       }
       steps{
          echo 'testing the project '
       }
    }
     stage("deploy"){
       steps{
          echo 'deploying the project '
       }
    }
  }
}
