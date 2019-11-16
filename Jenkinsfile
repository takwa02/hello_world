node {
        stage('Poll') {
            checkout scm
        }
        stage('Build') {
           withMaven(maven:'maven'){
                   mvn install}
        }
        stage('Test') {
            withMaven(maven:'maven'){ 
                    mvn test}
        }
        stage('Deploy') {
            withMaven(maven:'maven'){
                    mvn deploy}
        }
}
