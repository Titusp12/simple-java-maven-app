node('maven'){
    
    def maven360home = tool name: 'maven360', type: 'maven'
    
    stage('checkout'){
      git branch: 'batch2', credentialsId: 'bxnyy7github', url: 'https://github.com/Titusp12/simple-java-maven-app.git'
    }
    
    
    stage('Running Tests'){
        sh "$maven360home/bin/mvn clean test surefire-report:report-only"
    }
}
