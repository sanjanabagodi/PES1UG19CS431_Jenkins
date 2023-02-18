pipeline{
  agent any
  stages {
    stage('Build'){
      steps{
        git branch: 'main', url: 'https://github.com/sanjanabagodi/PES1UG19CS431_Jenkins.git'
        sh 'g++ -o program_output main/hello.cpp'
        echo 'Build Stage Successful'
      }
    }
    stage('Test'){
      steps{
        sh './program_outut'
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
