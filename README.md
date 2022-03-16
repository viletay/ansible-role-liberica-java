# Ansible Role: Install Liberica JDK from archive.

<<<<<<< HEAD
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
=======
[![License][license-image]][license-url] [![Ansible Galaxy][ansible-galaxy-image]][ansible-galaxy-url] [![Ansible Galaxy Quality][ansible-galaxy-quality-image]][ansible-galaxy-url] [![Ansible Galaxy Release][ansible-galaxy-release-image]][ansible-galaxy-url]
>>>>>>> 1665d7d0f3adf903c35adf6e7e6e021b7a68441a

 Install latest feature release or chosen release [Liberica JDK](https://bell-sw.com/) for Linux from archive.

 BellSoft Liberica JDK is a build of OpenJDK that is tested and verified to be compliant with the Java SE specification using OpenJDK Technology Compatibility Kit test suite for Linux, Windows, macOS, and Solaris operating systems.
 The distribution includes Server, Client, and Minimal JVMs.

 For more information, check out the [Liberica JDK product page](https://bell-sw.com/pages/libericajdk/)

## Work on

## Dependencies

min_ansible_version: 2.9

## Role Variables
```yaml
## Variable: liberica_java_home
#     Full pathname of a installation directory.
#
# Default:
# liberica_java_home: /usr/local/java
liberica_java_home: /usr/local/java

## Variable: liberica_java_version_feature
#     Specifies feature version or formerly known as a major version.
#
# Default:
# liberica_java_version_feature: 11
liberica_java_version_feature: 11

## Variable: liberica_java_bundle_type
#     Specifies the content of the package:
#         jdk      — a regular package that contains the full Liberica JDK, not including JavaFX.
#         jdk-full — contains the full Liberica JDK, including JavaFX and a variety of JVMs for platforms that support it.
#         jdk-lite — includes Liberica JDK with compressed modules and Server VM, without any extra packages.
#         jre      — contains Java SE Runtime Environment only.
#         jre-full — contains Java SE Runtime Environment, including JavaFX.
#     Please note that for Liberica JDK 8 there’re no lite packages.
#
# Default:
# liberica_java_bundle_type: jdk
liberica_java_bundle_type: jdk

## Variable: liberica_java_insecure
#     Allow the role to insert own java.security.
#
# Default:
# liberica_java_insecure: false
liberica_java_insecure: false

## Variable: liberica_java_version
#
#
#
#
#
