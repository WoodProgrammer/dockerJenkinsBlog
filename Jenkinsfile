node {
    
    stage("Git Checkout"){
     
        git credentialsId: '3af5981e-eb43-4b27-a774-e56d46eba935', url: 'https://github.com/WoodProgrammer/dockerJenkinsBlog'

    
    }
    stage("Build"){
        sh "docker build -t emirozbir/jdind:latest ."
        
    }
    
    stage("Docker push "){
        
        withCredentials([string(credentialsId: 'docker-pwd', variable: 'dockerHubLogin')]) {
                    sh "docker login -u emirozbir -p ${dockerHubLogin}"

        }
        sh "docker push emirozbir/jdind:latest"
        
    }
}
