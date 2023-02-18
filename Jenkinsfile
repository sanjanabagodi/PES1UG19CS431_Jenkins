pipeline{
  agent any
  stages {
    stage('Build'){
      steps{
        sh 'g++ -o sanjanabagodi/PES1UG19CS431_Jenkins/main/hello.cpp'
        echo 'Build Stage Successful'
      }
    }
    stage('Test'){
      steps{
        sh 'a.exe'
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
