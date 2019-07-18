node {
stage('Build'){
echo "build//"
}

stage('Slack notification'){
    slackSend channel: '#testing_slack',
    color: 'good',
    message: "*${currentBuild.currentResult}:* Job ${env.JOB_NAME} build ${env.BUILD_NUMBER}\n More info at: ${env.BUILD_URL}"
    }
}

