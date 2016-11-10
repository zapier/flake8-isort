#!groovy

node ('master'){
  stage 'Build and Test'
  sh 'pip install -e .'
  sh 'pip install pytest testfixtures'
  sh 'python run_tests.py'
}
