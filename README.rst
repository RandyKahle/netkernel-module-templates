This is the NetKernelROC community set of module templates that work with
and support the NetKernelROC NetKernel Gradle plugin.

Clone this repository and set the Gradle properties to reference the location.

For example, set your ~/.gradle/gradle.properties file to include::

  templateDirectory=/complete/path/to/this/repo
  templateLibrary=default

to use the default set of templates.

The structure of this repository is set to support many different libraries
of templates:

  /<library-name>/<template-name>

For example::

  /default/simple
  /databliss/standard
  /databliss/documentation
  /databliss/test
  /bestbuy/metis-standard

The Gradle plugin will copy the complete directory to a new NetKernel
module directory with the createNetKernelModules task.

Two variables are substituted (we might add more, please let us know)::

  MODULE_URI
  MODULE_CLASSPATH

Look at the module.xml file in default/simple to see how these variables
are used.

