node {
    environment {
        DISPLAY_BRANCH = sh ( script: "echo $branch|cut -d '/' -f 3", returnStdout:true).trim()
    }
    stage("Git Checkout"){
        
        
        currentBuild.displayName = "#${BUILD_NUMBER} - ${env.DISPLAY_BRANCH}"
    }
    stage("Build"){
        sh "docker build -t emirozbir/jdind:latest ."   
    }

}
