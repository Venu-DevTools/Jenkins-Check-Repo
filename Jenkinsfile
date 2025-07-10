pipeline {
    agent any


    stages {
        stage('Groovy Replace') {
            steps {
                script {
                         
                   def safeBranch = env.BRANCH_NAME.replaceAll('/', '_')

                    echo "Original Branch: ${env.BRANCH_NAME}"
                    echo "Mdified Branch (Groovy): ${safeBranch}"
                }
            }
        }
    }
}
