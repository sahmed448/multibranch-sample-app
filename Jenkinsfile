pipeline {
  
  agent { label "dev" };
  stages {
    stage('Hello') {
      steps {
        echo "hello"
      }
    }
    stage('for the dev branch') {
      when {
                branch 'dev' // Only run this stage for the 'dev' branch
            }
      steps {
        echo "this runs only for the dev"
      }
    }

    stage('for the prd') {
      when {
        branch 'prd'
      }
      steps {
        echo "this runs only for the prd"
      }
    }
    
  }
}
