pipeline {
    agent any
    environment{
    branch = "feature/CI/CD" 
    }

    stages {
        stage('Groovy Replace') {
            steps {
                script {
                         
                 //   def safeBranch = env.branch.replaceAll('/', '_') 
                      def safeBranch = env.BRANCH_NAME.replaceAll('/', '_')

                    echo "Original Branch: ${env.BRANCH_NAME}"
                    echo "Modified Branch (Groovy): ${safeBranch}"
                }
            }
        }
    }
}
