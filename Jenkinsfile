#!groovy

node ('master'){
  stage 'Build and Test'
  git url: 'https://github.com/gforcada/flake8-isort.git'
  sh 'virtualenv-2.7 .'
  sh 'bin/pip install -e .'
  sh 'bin/pip install pytest testfixtures'
  sh 'python run_tests.py'
}
