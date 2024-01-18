pipeline {
  agent { label 'slave1' }
stages {
  stage('checkout') {
    steps {
      sh 'rm -rf Parcel_service_feature-1'
      sh 'git clone https://github.com/Ahmsagar401/Parcel-service.git'
    }
  }
  stage('build') {
    steps {
      sh 'mvn --version'
      sh 'mvn clean install'
      sh 'mvn spring-boot:run'
    }
  }
}
}
