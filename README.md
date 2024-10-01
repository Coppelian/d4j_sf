To test this repository, you need to install defects4j: https://github.com/rjust/defects4j/tree/v2.1.0
When testing JDeodorant, please modify *.build.xml file in each directory.
Change the following part in this file to your repository.
<project name="" basedir="---Your base directory---">

    <taskdef resource="net/sf/antcontrib/antcontrib.properties">
        <classpath>
            <pathelement location="---this directory---/ant-contrib-1.0b3.jar"/>
        </classpath>
    </taskdef>
    <!-- CLI requires that local dependencies use the file:// prefix -->
    <property name="d4j.home" value="---Your d4j directory---/defects4j"/>
    <property name="d4j.workdir" value="---Your base directory---" />
    <property name="d4j.dir.projects" value="---Your d4j directory---/defects4j/framework/projects" />

After changing the file, you can load the projects into your eclipse to test.
