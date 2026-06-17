pipeline{
  agent any
  tools{
    gradle 'Gradle'
  }
  stages{
    stage('Checkout'){
      steps{
        git 'https://github.com/rakshitha-v1/myGradle.git'
      }
    }
    stage('Build'){
      steps{
        sh 'gradle build --stacktrace'
      }
    }
    stage('Run'){
      steps{
        sh 'gradle run'
      }
    }
  }
}
