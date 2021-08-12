pipeline {
  agent any
  // tools {
  //   maven 'maven 3.5.4'
  //   jdk 'JDK-1.8'
  // }
  stages {
    stage ('Build image') {
      steps {
        sh "docker build -t varidmahdi/laravel_cilsy:latest ."
        sh "docker push varidmahdi/laravel_cilsy:latest"
        sh "docker rmi varidmahdi/laravel_cilsy:latest"
      }
    }
  }
}