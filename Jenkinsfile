properties([parameters([choice(choices: ['build', 'test', 'deploy'], description: 'choose branch', name: 'branch')])])
pipeline {
    agent any 
  stages {
    stage ('build branch') {
      when {
                expression { branch == 'build'}
            }
            steps {
                echo "build is successful"
            }
    }
    stage ('test branch') {
      when {
                expression { branch == 'test'}
            }
            steps {
                echo "test sucessful!"
            }
    }
   stage ('deploy branch') {
      when {
                expression { branch == 'deploy'}
            }
            steps {
                echo "deploy successful"
            }
        }
  }
}
