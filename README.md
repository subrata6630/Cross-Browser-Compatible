# Cross-Browser-Compatible

Cross-browser means web application works with all versions of all browsers. To claim cross-browser compatibility, the website is nowadays expected to support browsers such as Mozilla Firefox,Google Chrome, Opera, and Safari in addition to Internet Explorer and Netscape. Here are the basic tips to make your website cross browser compatible.

1. Define Valid Doctype:
Your doctype tells the browser what rules you’ll be using in your code. If you don’t specify, the browser has to guess, and different browsers will guess differently. When you design in “strict mode,” Internet Explorer 6 and above will show behavior much closer to that of Firefox, Safari and other modern browsers.

<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01//EN"
 "http://www.w3.org/TR/html4/strict.dtd">
 

Otherwise, Internet Explorer runs in a “quirks mode” where it attempts to emulate the behavior of older browsers.

2. CSS Reset:
By default, Different browsers behave as per their default css rules. You need to explicitly define css to make same behavior for different browsers. I like Eric’s CSS reset:
http://meyerweb.com/eric/thoughts/2007/05/01/reset-reloaded/
http://meyerweb.com/eric/tools/css/reset/index.html

3. Conditional Comments:
Try to use conditional comments instead of CSS hacks.
With conditional comments you can link to separate style sheets for different browsers.

<link type="text/css" href="style.css" />
 <!--[If IE]>
 <link type="text/css" href="IEHacks.css" />
 <![endif]-->
 <!--[if !IE]>
 <link type="text/css" href="NonIEHacks.css" />
 <![endif]-->
 

4. Try to use javascript library like jQuery, YahooUI, MooTools, Dojo abstract away the differences in the DOM, AJAX and JavaScript.

5. You can use Css Frameworks like BluePrint, 960 Grid. These are mostly cross browser compatible.
See following to know which css framework is suitable for you.
http://net.tutsplus.com/tutorials/html-css-techniques/which-css-grid-framework-should-you-use-for-web-design/

6. Validate:
The W3C Validation Service validates multiple versions of XHTML and HTML, outputting many useful errors and warnings to help users create a perfect website.
W3C Validator: http://validator.w3.org/
W3C Css Validator: http://jigsaw.w3.org/css-validator/

7. Testing: 
I would suggest you to start with firefox and then move to IE. Use Firebug, a firefox addon and IE Developer Toolbar for IE to set layout. To test website on different browser, there are some online and offline utilities like
browsershots,
IETester,
browsercam.

See following to get more app for testing cross browser compatibility:

http://designm.ag/resources/cross-browser-testing/
http://www.bestpsdtohtml.com/7-awesome-resources-to-test-cross-browser-compatibility-of-your-website/

If you are designer you must know difference between different browsers. For this, See followings:

http://www.iecss.com/
http://www.smashingmagazine.com/2009/10/14/css-differences-in-internet-explorer-6-7-and-8/

If you use other ways to make your site cross browser compatible, please leave a comment and share it. If you liked this article don’t forget to digg or share it.
