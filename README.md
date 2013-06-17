
Runs JDepend metrics on your Griffon application
------------------------------------------------

Plugin page: [http://artifacts.griffon-framework.org/plugin/jdepend](http://artifacts.griffon-framework.org/plugin/jdepend)


Provides code metrics with [JDepend][1]. JDepend traverses Java class file directories and generates design
quality metrics for each Java/Groovy package. JDepend allows you to automatically measure the quality of a
design in terms of its extensibility, reusability, and maintainability to manage package dependencies effectively. 

Usage
-----

Just execute the `jdepend` command target.

Configuration
-------------

The plugin will automatically exclude the following packages 

 * `java.lang`
 * `java.util`
 * `java.net`
 * `java.io`,
 * `java.math`
 * `groovy.lang`
 * `groovy.util`
 * `org.codehaus.groovy.*`
 
You can specify additional exclusions by defining the following property on `BuildConfig.groovy`

        griffon.jdepend.excludes = ['package.one', 'package.two']

Scripts
-------

 * **jdepend** - run jdepend metrics on the application's source code

[1]: http://clarkware.com/software/JDepend.html

