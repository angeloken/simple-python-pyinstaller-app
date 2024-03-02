node {
    stage('Build') {
        checkout scm // Assuming you're using a Git repository
        sh 'python -m py_compile sources/add2vals.py sources/calc.py'
        stash name: 'compiled-results', includes: 'sources/*.py*'
    }
}