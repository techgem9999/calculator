pipeline{
agent any
stages{
stage('checkout'){
steps{
   checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/techgem9999/calculator.git']]])
   }}
    stage('compile'){
    steps{
        sh '/opt/apache-maven-3.6.0/bin/mvn compile'
    }}
   }}
