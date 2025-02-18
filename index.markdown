---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---

# Introducing Syphon

Syphon is an [open source](http://github.com/syphon) Mac OS X technology that allows applications to share frames - full frame rate video or stills - with one another in realtime. Now you can leverage the expressive power of a plethora of tools to mix, mash, edit, sample, texture-map, synthesize, and present your imagery using the best tool for each part of the job. Syphon gives you flexibility to break out of single-app solutions and mix creative applications to suit your needs.


# Features

Syphon provides an ecosystem for sharing imagery between applications and new media development environments. Syphon is designed to be efficient and will not duplicate resources unnecessarily, keeping your frame rate and best interests in mind.

* Hardware accelerated surface sharing on the GPU where it belongs. 
* Zero latency.
* Zero copy.
* Support arbitrary resolutions up to your GPU's limit. Typically 16k x 16k.
* Support abritrary frame rates.
* Support alpha-channels.
* Compatible with MacOS X 10.6 (Snow Leopard) or later.
* Compatible with Legacy OpenGL, Core Profile OpenGL, and Metal back ends.
* Interoperable between renderers. Share frames between OpenGL and Metal Renders out of the box.
* A simple SDK so developers can add Syphon to just about any application.

# Applications

The list of Syphon enabled applications keeps growing. Here are is a sample of interoperable applications, inlcuding live performance, content creation, show control, visualizers, development, creative coding, live coding, patching environments, game engines, projection mapping, capture tools and broadcast playout.

You can mix these tools and more to find unique solutions to your creative problems.


<div align="center" style="margin-bottom:20px; margin-top:20px">

{% for app in site.hero_apps %}

<a href="{{ app.website }}"><img src="app_icons/{{app.icon}}" width="128" height="128" style="padding:10px"></a>

{% endfor %}

</div>


<div align="center" style="margin-bottom:20px; margin-top:20px">

{% for app in site.apps %}

<a href="{{ app.website }}" title="{{app.title}}"><img src="app_icons/{{app.icon}}" width="45px" height="45px" style="padding:20px"></a>

{% endfor %}

</div>

# Developer SDK


* ![SDK](app_icons/Xcode_icon.png "SDK") [Syphon.framework](https://github.com/Syphon/Syphon-Framework) allows 3rd party developers to leverage frame-sharing in their applications or plugins. A simple Objective-C interface allows the publishing and acquisition of frames in very few lines of code. Under the hood, Syphon uses the power of IOSurface plus a selection of Cocoa and Core Foundation technologies to manage the communication between servers and clients. [Download](http://github.com/Syphon/Syphon-Framework). [Developer Documentation](/FrameworkDocumentation)

* ![Syphon Client and Server](app_icons/Syphon_32.png "Syphon Client and Server") [Simple Server/Client](https://github.com/Syphon/Simple) A pair of applications to test Syphon functionality (download)


If you’d like to get involved, join us at the [GitHub projects](http://github.com/Syphon) for the framework and implementations.


# Proudly Sponsored By

<div align="center" style="margin-bottom:20px; margin-top:20px">

{% for sponsor in site.sponsors %}

<a href="{{ sponsor.website }}" title="{{sponsor.title}}"><img src="sponsors/{{sponsor.icon}}" width="128" height="128" style="padding:10px"></a>

{% endfor %}

	<form action="https://www.paypal.com/cgi-bin/webscr" method="post">
	<input 	type="hidden" name="cmd" value="_s-xclick">
		<input type="hidden" name="hosted_button_id" value="C98K2YZNQ8YSW">
		<input type="image" src="https://www.paypal.com/en_US/i/btn/btn_donate_SM.gif" border="0" name="submit" alt="PayPal - The safer, easier way to pay online!">
		<img alt="" border="0" src="https://www.paypal.com/en_US/i/scr/pixel.gif" width="1" height="1">
	</form>

</div>
Syphon is designed for and by new media technologists, realtime video artists and visualists. It is a labor of love, developed in the spare time of the authors. It is open, free and a gift to the new media community. If Syphon is useful to you or an application you are developing, please consider contributing or sponsoring to help continue development and support the cause.



# Contact and Support

Some common questions are answered in our [FAQ](/faq). If you have questions about a product which integrates Syphon, please contact the developer of that produce for support. Developers can report issues or request features for the [Syphon framework on GitHub](https://github.com/Syphon/Syphon-Framework/).


# Authors

Syphon.framework, test suite, and initial implementations are written by [Tom Butterworth](http://kriss.cx/tom) and [Anton Marini](https://vade.info) with major support from [Vidvox](http://vidvox.com) and Metal implementation input from [Millumin](www.millumin.com)

# License

Syphon.framework, test suite, and our provided reference implementations are [licensed under a Simplified BSD software license](/license).
