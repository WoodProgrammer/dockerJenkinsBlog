node {
    
    stage("Git Checkout"){
        sh "echo testimtest"
        git credentialsId: '3af5981e-eb43-4b27-a774-e56d46eba935', url: 'https://github.com/WoodProgrammer/dockerJenkinsBlog'
    }
    stage("Build"){
        sh "docker build -t emirozbir/jdind:latest ."   
    }

}
