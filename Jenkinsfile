pipeline{
  agent any
  stages {
    stage('Build'){
      steps{
        sh 'build PES1UG19CS431-1'
        echo 'Build Stage Successful'
      }
    }
    stage('Test'){
      steps{
        echo 'Test Stage Successful'        
      }
    }
    stage('Deploy'){
      steps{
        echo 'Deployment Stage Successful'        
      }
    }
  }
  post{
    failure{
      echo 'Pipeline failed'
    }
  }
}
