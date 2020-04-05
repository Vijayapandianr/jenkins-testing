pipeline {
    agent any

    stages {
        stage('Parallel') {
            parallel {
        
        stage ('satge one') {
           when {
         expression {
                return env.BRANCH_NAME == 'develop';
            }
        }
            steps {
                 
                echo 'stage one'
                }
            }
        

        stage ('Second Stage') {

            steps {
                input message: 'Approve Deploy?', ok: 'Yes'
                echo 'stage one'
                }
            }
        


        stage ('Deployment Stage') {
            steps {
               echo 'Deployment'
            }
        }
    }
        }
    }
}
