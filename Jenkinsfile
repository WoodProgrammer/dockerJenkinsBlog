node {
    DISPLAY_BRANCH = sh ( script: "echo $branch|cut -d '/' -f 3", returnStdout:true).trim()
    stage("Git Checkout"){
        
        
        currentBuild.displayName = "#${BUILD_NUMBER} - ${DISPLAY_BRANCH}"
    }
    stage("Build"){
        sh "echo New Branch"   
        sh "echo New Branch"   
        sh "echo New Branch"   
        sh "echo New Branch"   

    }

}
