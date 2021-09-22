# How to make a Hello on OSGi with IntelliJ

Before starting we need to understand a little bit what OSGi is.

- OSGi  stands for Open Services Gateway initiative
- Specification and set of standard for module software development with Java 
- Products using OSGi: Eclipse, GlassFish, Jira, Liferay and many...

I'll leave some links that helped you understand what OSGi

### Let's start

- Download [Apache Felix](http://felix.apache.org/)
- Dependency [OSGi Framework](https://mvnrepository.com/artifact/org.osgi/org.osgi.framework/1.8.0)

1. Open IntelliJ and create a new project. It's up to you which build tool you use. I will use Gradle. Click on File -> New Project -> Choose Gradle and then Java -> Project Name: hello-osgi -> Finish
2. Let's add the [OSGi plugin](https://plugins.jetbrains.com/plugin/1816-osgi) or open your IntelliJ and click on `File` -> `Settings` -> `Plugins` -> Choose `Marketplace` and search for `OSGi`, install the plugin and apply. 
3. On the left side under plugin go to Languages & Frameworks -> OSGi -> Add to framework instances you downloaded (Apache Felix). When you select the Felix folder, the system will recognize the Felix version and click OK.
4. On the upper right side, click Edit configurations -> Add -> OSGi Bundles -> OSGi Bundles Name -> Select the OSGi Framework that will show the felix that was already configured in step 3, let's click on the parameters tab -> use this directory and select the folder where the project will be built (/hello-osgi/build/libs) and click OK.
5. You can start the OSGi Bundles and you will have the Gogo Shell terminal, you can use the lb command to list all bundles. Now let's write our code.

## To be continued...

    