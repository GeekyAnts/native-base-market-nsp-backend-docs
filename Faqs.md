# FAQs


- [How to override style in NativeBase?](#override-style)
- [How do I add events with the components?](#add-events)
- [None of the above, I have a different error](#none)
- [How to customize components of NativeBase?](#customize)
- [I want list of icons with their names used in NativeBase](#list-icons)
- [How do I extract files in Windows?](#windows-extraction)
- [How to eject CRNA to get regular React Native app?](#CRNA-ejection)

<br />
<hr />

<a id="override-style"></a>
#### How to override style in NativeBase?

<div id="faq-5" class="panel-collapse collapse">
    <div class="panel-body">
        I didn't find a way to override style. <br />
        How can I include React StyleSheet into my app?
    </div>
    <br />
    <div class="panel-footer">
        <b> Solution: </b><br />
        <a href="http://nativebase.io/">NativeBase</a> is built on top of <a href="https://facebook.github.io/react-native/">React Native</a>.<br />
        Hence with any component, you can pass the style property which will be merged into the default style of that component.<br />

        Example:
        <pre><code class="language-jsx">&lt;Button style=&#123;{backgroundColor: '#FF0000'}}>
        Click me!&lt;/Button></code></pre>
    </div>
</div>

<br />
<hr>

<a id="add-events"></a>
#### How do I add events with the components?

<div id="faq-6" class="panel-collapse collapse">
    <div class="panel-body">
        What events are available for the components?<br />
        Example buttons, list items etc.
    </div>
    <br />
    <div class="panel-footer">
        <b>Solution:</b> <br />
        The <a href="http://nativebase.io/">NativeBase</a> components are built on top of <a href="https://facebook.github.io/react-native/">React Native</a> components. Hence the callback events of React Native holds good with NativeBase components. <br />

        <i>Example:</i> The <code>Button</code> component is actually a wrapper of the <code>TouchableOpacity</code> component of React Native. So you can just use the <code>onPress</code> callback function for event handling.<br /><br />

        Refer the
        <a href="http://docs.nativebase.io/">cheatsheet</a>
        for more details.
    </div>
</div>

<br />
<hr>

<a id="none"></a>
#### None of the above, I have a different error


<div id="faq-7" class="panel-collapse collapse">
    <div class="panel-body">
        The above-listed FAQs were not of your help?<br />
        Facing some other issues?
    </div>
    <br />
    <div class="panel-footer">
        <b>Solution:</b> <br />
        We welcome all your issues. Feel free to raise issues on GitHub.<br />
        Please go to the <a href="">Git Flow</a> to report issues.
    </div>
</div>

<br />
<hr>

<a id="customize"></a>
#### How to customize components of NativeBase?

<div id="faq-8" class="panel-collapse collapse">
    <div class="panel-body">
        I didn't find a way to customize the default styles of NativeBase components. <br />
    </div>
    <br />
    <div class="panel-footer">
        <b> Solution: </b><br />
        <a href="http://nativebase.io/">NativeBase</a> provides a separate file inclusive of color schemes for all components.<br />
        Go through <a href="http://docs.nativebase.io/CUSTOMIZE.html#Customize">Customize</a> section of docs.
    </div>
</div>

<br />
<hr>

<a id="list-icons"></a>
#### I want list of icons with their names used in NativeBase

<div id="faq-9" class="panel-collapse collapse">
    <div class="panel-body">
        Docs says <b>Choose from 700+ Icons</b><br />
        I want the complete list of icons containing the name and image of the icons that are ready to use.
    </div>
    <br />
    <div class="panel-footer">
        <b> Solution: </b><br />
        NativeBase uses Icons from <a href="https://expo.github.io/vector-icons/">React Native Vector Icons</a>.<br />
        Hence the collection of icons from Vector Icons holds good with that in NativeBase.
    </div>
</div>

<br />
<hr>

<a id="windows-extraction"></a>
#### How do I extract files in Windows?

<div id="faq-10" class="panel-collapse collapse">
    <div class="panel-body">
     I want to extract files in Windows.   
    </div>
    <br />
    <div class="panel-footer">
        <b> Solution: </b><br />
        • Unzip the file.<br />
        • Right click on the extracted file and select <b>View files</b>.<br />
        All the files will be extracted.<br /><br />


        <b> NOTE: </b>We don't provide support for Windows. It's completely buyer's responsibility.
    </div>
</div>

<br />
<hr>
<a id="CRNA-ejection"></a>
#### How to eject CRNA to get regular React Native app?

<div id="faq-11" class="panel-collapse collapse">
    <div class="panel-body">
     I want to eject from CRNA to get regular React Native app.   
    </div>
    <br />
    <div class="panel-footer">
        <b> Solution: </b><br />
        Ejecting from CRNA to regular React Native app can be performed referring this <a href="https://github.com/react-community/create-react-native-app/blob/master/EJECTING.md">link</a>.
    </div><br />However, we don't recommend to eject it fully as we have used few features that are dependent on ExpoKit . So if you plan to eject it you can partially eject it and use the app with ExpoKit.
<hr>

