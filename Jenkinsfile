pipeline{
agent any
stages{
    stage('Docker login'){
        steps{
            sh 'docker login -u sayan556 -p Sayanm15@'
        }
        
    }
    stage('Docker image build'){
        steps{
            sh 'docker build -t sayan-exam .'
            sh 'docker images'
        }
        
    }
    stage('Tag docker image'){
        steps{
            sh 'docker tag sayan-exam sayan556/examrepo:newimage'
        }
        
    }
    stage('Push docker image'){
        steps{
            sh 'docker push sayan556/examrepo:newimage'
        }
        
    }
}
}
