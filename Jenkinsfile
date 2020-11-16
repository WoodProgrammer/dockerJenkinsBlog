node {
    
    stage("Git Checkout"){
        BRANCH = sh ( script: "echo $branch|cut -d '/' -f 3", returnStdOut:true)
        
        currentBuild.displayName = "#${BUILD_NUMBER} - ${BRANCH}"
    }
    stage("Build"){
        sh "docker build -t emirozbir/jdind:latest ."   
    }

}
