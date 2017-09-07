# libwsdl4j-java-maven Debian package

Official libwsdl4j-java Debian package installs .jar-s only into `/usr/share/java`, but not into local Maven repo (`/usr/share/maven-repo`).

The current package simply depends on `libwsdl4j-java` and creates necessary symlinks and .pom files in Debian local Maven repo. So, for example, `wsdl4j:wsdl4j:debian` gets available from the local Maven repo if `libwsdl4j-java-maven` is installed.
