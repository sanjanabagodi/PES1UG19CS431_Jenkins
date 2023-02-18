pipeline{
  agent any
  stages {
    stage('Build'){
      steps{
        sh 'g++ -o https://github.com/sanjanabagodi/PES1UG19CS431_Jenkins/tree/main/main/hello.cpp'
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
