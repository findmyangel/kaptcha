&lt;wiki:gadget url="http://kaptcha.googlecode.com/svn/wiki/adsense3.xml" border="0" width="470" height="60" /&gt;

&lt;wiki:gadget url="http://kaptcha.googlecode.com/svn/wiki/donate.xml" border="0" width="150" height="75" /&gt;

### Q: kaptcha images do not show up on my linux box! What's going on? ###

It **may** be because you are using GNU java. Try running:

`java -version`

from the console. If it mentions GNU, then kaptcha will not produce an image. To fix it, simply download and install a Sun JDK and make sure that its bin directory comes before the GNU java in the path.

Note that this is likely to occur with Ubuntu and OpenSUSE. Other distributions probably package GNU java as well, but these two are confirmed.

### Q: How do I remove the image distortion? ###

```
package com.mine;
public class NoDistortion implements GimpyEngine {
       @Override
       public BufferedImage getDistortedImage(BufferedImage bi) {
               return bi;
       }
}
```

And in your servlet definition:
```
<init-param>
     <param-name>kaptcha.obscurificator.impl</param-name>
     <param-value>com.mine.NoDistortion</param-value>
</init-param>
```

### Q: What is the difference between kaptcha-2.3-jdk14.jar and kaptcha-2.3.jar? ###

The only difference is that you should use the jdk14 jar if you are using jdk14.

### Q: How should I configure my own colors? ###

r,g,b:

```
<init-param>
    <param-name>kaptcha.noise.color</param-name>
    <param-value>0,0,255</param-value>
</init-param>
```

### Q: java.lang.NoClassDefFoundError: Could not initialize class sun.awt.X11GraphicsEnvironment ###

When starting up the JVM, add the parameter:
```
-Djava.awt.headless=true
```

This article also looks good: http://www.fromdev.com/2010/06/how-to-solve-kaptcha-error-on-glassfish.html
&lt;wiki:gadget url="http://kaptcha.googlecode.com/svn/wiki/donate.xml" border="0" width="150" height="75" /&gt;