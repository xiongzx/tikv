#!groovy

node {
    def TIDB_TEST_BRANCH = "master"
    def TIDB_BRANCH = "rc4"
    def PD_BRANCH = "rc4"

    fileLoader.withGit('git@github.com:pingcap/SRE.git', 'master', 'github-iamxy-ssh', '') {
        fileLoader.load('jenkins/ci/pingcap_tikv_branch.groovy').call(TIDB_TEST_BRANCH, TIDB_BRANCH, PD_BRANCH)
    }
}
