#!groovy

node {
    def TIDB_TEST_BRANCH = "master"
    def TIKV_BRANCH = "shirly/dag_expression"
    def PD_BRANCH = "master"

    fileLoader.withGit('git@github.com:pingcap/SRE.git', 'master', 'github-iamxy-ssh', '') {
        fileLoader.load('jenkins/ci/pingcap_tidb_branch.groovy').call(TIDB_TEST_BRANCH, TIKV_BRANCH, PD_BRANCH)
    }
}
