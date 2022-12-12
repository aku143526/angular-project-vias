node {
    stage('Checkout SCM') {
        git branch: 'main', url: 'https://github.com/aku143526/angular-project-vias.git'
    }
 
    stage("Install node modules"){
        sh "npm install"
            
    }
   
    stage("Build"){
        sh "ng build"
    }
      
    stage("Deploy"){
       sh "npm run build --prod"
    }
  
}
