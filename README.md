# Maven Repo
This is the public Maven repository for Lemniscate projects. 

Todo: Document usage.


### Installing a project to the local repository **for RELEASE**
`mvn -DaltDeploymentRepository=snapshot-repo::default::file:/Users/$USER/workspace/oss/lemniscate-maven-repo/releases clean deploy`
### Installing a project to the local repository **as a snapshot**
`mvn -DaltDeploymentRepository=snapshot-repo::default::file:/Users/$USER/workspace/oss/lemniscate-maven-repo/snapshots clean deploy`
