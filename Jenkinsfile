pipeline{
    agent any
    tools {
        maven "weshopify-platform-maven"
    }
    stages{
        stage('pull the source code'){
            steps{
                echo 'pulling the source code'
                git branch: 'security', url: 'https://github.com/NarsiMyTeaching/weshopify-platform-monolith-app.git'
                echo '==============================='
                echo 'source code pulling completed'
                echo '==============================='
            }
        }
        stage('building the source code'){
            steps{
                echo 'building the code using maven build tool'
            }
        }

        stage ('pushing the artifact to jfrog artifactor'){
            steps{
                echo "pushing the artifact to Jfrog Artifactory"
            }
        }
    }
}