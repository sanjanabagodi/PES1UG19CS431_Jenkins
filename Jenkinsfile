pipeline{
  agent any
  stages {
    stage('Clone repository') {
      steps {
        git branch: 'main', url: 'https://github.com/sanjanabagodi/PES1UG19CS431_Jenkins.git'
      }
    }
    stage('Build'){
      steps{
        sh 'g++ -o program_output main/hello.cpp'
        echo 'Build Stage Successful'
      }
    }
    stage('Test'){
      steps{
        sh './program_output'
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
