node('my-openshift-build') {

    def mvnReturnStatus = 0
    def pomVersion = '0.0.0'
    try {
        stage('checkout source code') {
            checkout scm
        }

    } catch (Exception e) {
        println e
        currentBuild.result = 'FAILED'
    }
}