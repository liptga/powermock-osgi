# About
Powermock is a popular mocking framework (https://code.google.com/p/powermock) which can be used to mock classes or methods which otherwise can not be mocked. This project is about to enable its use in OSGI environments especially using it for testing Eclipse Plugins.

# How to use
Simply add one of the desired features to your target platform using the latest update site.

# How to build
```
powermock-osgi> mvn clean install
powermock-osgi/p2> mvn clean install
```

# Latest Version
The latest version is based on 1.5.6 Powermock. Update site: https://raw.githubusercontent.com/liptga/powermock-osgi/master/update-site/1.5.6.0 . 
See the release notes.

# Disclaimer
I tested ONLY the Junit+Mockito+Powermock feature. The others should also work, but I did not test them.

# Useful Trick
Known limitation is that Powermock can play only with classes in exported packages, but it is usually enough. It is possible however to export some packages only for usage of powermock using the x-friends manifest entry. See http://blog.vogella.com/2010/05/25/x-friends-in-equinox/.
        