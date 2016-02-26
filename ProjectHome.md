![https://kaptcha.googlecode.com/svn/wiki/images/blockchain.png](https://kaptcha.googlecode.com/svn/wiki/images/blockchain.png)

&lt;wiki:gadget url="http://kaptcha.googlecode.com/svn/wiki/adsense3.xml" border="0" width="475" height="60" /&gt;

### Introduction ###

By default, Kaptcha is very easy to setup and use and the default output produces a captcha that should be fairly hard to bust. The captcha's it produces by default look very similar to the one above. If you would like to change the look of the output, there is several configuration options and the framework is modular so you can write your own morphing code.

If you have a valid issue with the functionality or design of kaptcha, please click the [Issues tab](http://code.google.com/p/kaptcha/issues/list) and file one.

**I've spent a lot of time on this project. Donations are welcome and very much appreciated.**

Bitcoin: 14fsfnCMMMg8NHFx4vQdAzNwquJoiwSrYB

<table border='0'>
<tr>
<td>
<wiki:gadget url="http://kaptcha.googlecode.com/svn/wiki/donate.xml" border="0" width="150" height="70" /><br>
</td>
<td>
<wiki:gadget url="http://www.ohloh.net/p/4850/widgets/project_users_logo.xml" height="43" border="0"/><br>
</td>
<td>
<wiki:gadget url="http://www.ohloh.net/p/4850/widgets/project_thin_badge.xml" height="36" border="0"/><br>
</td>
</tr>
</table>

### Changes ###
**unreleased** -
  * Only set session attributes after the image is written out, in case that fails. [Issue #69](https://code.google.com/p/kaptcha/issues/detail?id=#69)

**v2.3.2** - December 5, 2010
  * Fix small bug introduced in 2.3.1 where not all characters were being added to the image. [Issue #37](https://code.google.com/p/kaptcha/issues/detail?id=#37)

**v2.3.1** - November 20, 2010
  * [All fixes are in the issue tracker](http://code.google.com/p/kaptcha/issues/list?can=1&q=status%3Afixed+milestone%3A2.3.1&colspec=ID+Type+Status+Priority+Milestone+Owner+Summary&cells=tiles)

**v2.3** - July 25, 2008
  * [All fixes are in the issue tracker](http://code.google.com/p/kaptcha/issues/list?can=1&q=status%3Afixed+milestone%3A2.3&colspec=ID+Type+Status+Priority+Milestone+Owner+Summary&cells=tiles)

**v2.2** - Mar 21, 2008
  * [Added Unit Tests](http://code.google.com/p/kaptcha/issues/detail?id=9&can=1)
  * [Fixed bug with ShadowGimpy config](http://code.google.com/p/kaptcha/issues/detail?id=10&can=1)
  * [Use JavaIO to generate the images](http://code.google.com/p/kaptcha/issues/detail?id=11&can=1)
  * Send all recommended no-cache http headers
  * Bit more code refactoring and cleanup.

**v2.1** - Feb 15, 2008
  * Upgraded to Retroweaver 2.0.4.
  * Fixed issue with build system.
  * Reformatted all the source code.
  * Applied the [patch from cliffano](http://code.google.com/p/kaptcha/issues/detail?id=5) that refactored the configuration and various other cleanup. I changed his configuration patch a bit as well.
  * Deleted SimpleKaptcha servlet as it was unnecessary, unmaintained and had several usage issues.
  * Add no caching and content type response headers to KaptchaServlet

**v2.0** - Oct 2, 2007
  * Upgraded to Retroweaver 2.0.1.
  * Mass code cleanup and refactoring.
  * Provide documentation for the web.xml init parameters. @see ConfigParameters.
  * A couple small bugs have been fixed.

**v1.2**
  * JDK 1.4 is supported by adding Retroweaver support to the build system and a jdk1.4 jar is included with the distribution.

**v1.1**
  * Re-organized code a whole lot. Moved and renamed a lot of files. The code layout is much more clear now.
  * Removed all references to 'simple' in the Constants.

**v1.0**
  * Re-organized code a bit.
  * Added Eclipse project files.
  * Removed a bunch of duplicate and unused code.
  * Zero warnings/errors in Eclipse.
  * Rewrote the ant build file.

&lt;wiki:gadget url="http://kaptcha.googlecode.com/svn/wiki/adsense3.xml" border="0" width="468" height="60" /&gt;