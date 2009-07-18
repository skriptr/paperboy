# Paperboy

Paperboy is a mail sending library for the [Joyent Smart Platform](http://smart.joyent.com/) that uses the execution queue in order to provide non-blocking email delivery to multiple platforms. New platforms can be easily added IF AND ONLY IF they have a web API (currently a limitation of the platform). Make sure to configure your platform and authentication credentials for paperboy at the beginning of your 'bootstrap.js' file.

## Install

Add Paperboy as a git submodule. In the root of your your smart project run:

    git submodule add git://github.com/voodootikigod/paperboy.git js/paperboy
    
**Or** if you would like to contribute back to paperboy, fork the project and then install the submodule with your remote repo location:

    git submodule add git@github.com:<username>/paperboy.git js/paperboy
    
## Usage

In your 'bootstrap.js' file tell your smart application to use Paperboy:
    
    system.use("paperboy.init")