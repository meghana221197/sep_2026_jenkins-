pipeline {
    agent any

    parameters {
        string(defaultValue: 'main', description: 'Provide the branch to build and deploy', name: 'BRANCH')
        
        choice(choices: ['TEST', 'QA', 'PRE-PROD', 'PROD'], 
               description: 'Choose env to deploy ', 
               name: 'ENVIRONMENT')

        booleanParam defaultValue: true, description: 'Un check this to actually deploy', name: 'DRY-RUN'
    }

    stages {
        stage('STAGE1') {
            steps {
                sh '''
                    echo "BRANCH: $BRANCH"
                    echo "ENVIRONMENT: $ENVIRONMENT"
                    echo "DRY-RUN: $DRY-RUN"

                '''
                   echo "BRANCH: ${params.BRANCH}"
                    echo "ENVIRONMENT:${params.ENVIRONMENT}"
                    echo "DRY-RUN: ${params.DRY-RUN}"
            }
        }

    }
}