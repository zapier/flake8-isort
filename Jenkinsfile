#!groovy

node ('master'){
  stage 'Build and Test'
  sh 'virtualenv-2.7 .'
  sh 'bin/pip install -e .'
  sh 'bin/pip install pytest testfixtures'
  sh 'bin/python run_tests.py'
}
