pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'echo "Hello world!"'
            }
        }
    }
}
        def changeLogSets = currentBuild.changeSets
        for (int i = 0; i < changeLogSets.size(); i++) {
        def entries = changeLogSets[i].items
        for (int j = 0; j < entries.length; j++) {
        def entry = entries[j]
        def files = new ArrayList(entry.affectedFiles)
        for (int k = 0; k < files.size(); k++) {
        def file = files[k]
        //echo "${file.editType.name} ${file.path}"
        //echo  "${file.path}"
        echo "${file}"
           }
        }
     }
