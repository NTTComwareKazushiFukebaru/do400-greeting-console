pipeline{
    agent{
        label "nodejs"
    }
    stages{
        stage("Install dependencies"){
            steps{
                sh "npm ci"
            }
        }

        stage("Check Style"){
            steps{
                sh "npm run lint"
            }
        }

        stage("Test"){
            steps{
                sh "npm test"
            }
        }

        // Add the Release stage here
<<<<<<< HEAD
=======
stage('Release') {
steps {
sh '''
oc project vtbyyv-greetings
oc start-build greeting-console --follow --wait
'''
}
}
>>>>>>> a979dc9... Initial
    }
}
