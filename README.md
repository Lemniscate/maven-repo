# Maven Repo
This is the public Maven repository for Lemniscate projects. 

## Get Started

Simply add these repositories to your maven project, then import the projects as needed. 
```
    <repositories>
        <repository>
            <id>lemniscate-repo</id>
            <url>https://github.com/lemniscate/maven-repo/raw/master/releases</url>
        </repository>
        <repository>
            <id>lemniscate-snapshot-repo</id>
            <url>https://github.com/lemniscate/maven-repo/raw/master/snapshots</url>
            <snapshots>
            </snapshots>
        </repository>
    </repositories>
```

## Developer Notes

### Installing a project to the local repository **for RELEASE**
`mvn -DaltDeploymentRepository=snapshot-repo::default::file:/Users/$USER/workspace/oss/lemniscate-maven-repo/releases clean deploy`
### Installing a project to the local repository **as a snapshot**
`mvn -DaltDeploymentRepository=snapshot-repo::default::file:/Users/$USER/workspace/oss/lemniscate-maven-repo/snapshots clean deploy`
