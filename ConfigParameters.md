&lt;wiki:gadget url="http://kaptcha.googlecode.com/svn/wiki/adsense3.xml" border="0" width="470" height="60" /&gt;

# Introduction #

&lt;wiki:gadget url="http://kaptcha.googlecode.com/svn/wiki/donate.xml" border="0" width="150" height="75" /&gt;

Configuration is done through web.xml. All values can be left blank and a default value will be chosen.

Below is an example of the init-param you would add to your web.xml. If you want to set other variables, then you would add more init-param blocks.

```
<init-param>
    <param-name>kaptcha.border</param-name>
    <param-value>yes</param-value>
</init-param>
```

Note: This only works with the KaptchaServlet. SimpleServlet does not pay attention to the web.xml parameters.

# Details #

These values are stored in the `com.google.code.kaptcha.Constants` class.

| **Constant** | **Description** | **Default** |
|:-------------|:----------------|:------------|
| kaptcha.border | Border around kaptcha. Legal values are yes or no. | yes         |
| kaptcha.border.color | Color of the border. Legal values are r,g,b (and optional alpha) or white,black,blue. | black       |
| kaptcha.border.thickness | Thickness of the border around kaptcha. Legal values are > 0. | 1           |
| kaptcha.image.width | Width in pixels of the kaptcha image. | 200         |
| kaptcha.image.height | Height in pixels of the kaptcha image. | 50          |
| kaptcha.producer.impl | The image producer. | com.google.code.kaptcha.impl.DefaultKaptcha |
| kaptcha.textproducer.impl | The text producer. | com.google.code.kaptcha.text.impl.DefaultTextCreator |
| kaptcha.textproducer.char.string | The characters that will create the kaptcha. | abcde2345678gfynmnpwx |
| kaptcha.textproducer.char.length | The number of characters to display. | 5           |
| kaptcha.textproducer.font.names | A list of comma separated font names. | Arial, Courier |
| kaptcha.textproducer.font.size | The size of the font to use. | 40px.       |
| kaptcha.textproducer.font.color | The color to use for the font. Legal values are r,g,b. | black       |
| kaptcha.textproducer.char.space | The space between the characters | 2           |
| kaptcha.noise.impl | The noise producer. | com.google.code.kaptcha.impl.DefaultNoise |
| kaptcha.noise.color | The noise color. Legal values are r,g,b. | black       |
| kaptcha.obscurificator.impl | The obscurificator implementation. | com.google.code.kaptcha.impl.WaterRipple |
| kaptcha.background.impl | The background implementation. | com.google.code.kaptcha.impl.DefaultBackground |
| kaptcha.background.clear.from | Starting background color. Legal values are r,g,b. | light grey  |
| kaptcha.background.clear.to | Ending background color. Legal values are r,g,b. | white       |
| kaptcha.word.impl | The word renderer implementation. | com.google.code.kaptcha.text.impl.DefaultWordRenderer |
| kaptcha.session.key | The value for the kaptcha is generated and is put into the HttpSession. This is the key value for that item in the session. | KAPTCHA\_SESSION\_KEY |
| kaptcha.session.date | The date the kaptcha is generated is put into the HttpSession. This is the key value for that item in the session. | KAPTCHA\_SESSION\_DATE |

&lt;wiki:gadget url="http://kaptcha.googlecode.com/svn/wiki/donate.xml" border="0" width="150" height="75" /&gt;

&lt;wiki:gadget url="http://kaptcha.googlecode.com/svn/wiki/adsense3.xml" border="0" width="470" height="60" /&gt;