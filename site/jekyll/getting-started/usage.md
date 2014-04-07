---
layout: docs
title: Basic Usage
---

Once installed, create your React components as usual, ensuring you add the
`/** @jsx React.DOM */` docblock.

```javascript
// /Scripts/HelloWorld.jsx
/** @jsx React.DOM */
var HelloWorld = React.createClass({
	render: function () {
		return (
			<div>Hello {this.props.name}</div>
		);
	}
});
```

On-the-Fly JSX to JavaScript Compilation
----------------------------------------
Hit a JSX file in your browser (eg. `/Scripts/HelloWorld.jsx`) and observe
the magnificence of JSX being compiled into JavaScript with no precompilation
necessary.

Next Steps
-----------
On-the-fly JSX compilation is good for fast iteration during development, but
for production you will want to precompile for best performance. This can be
done via [ASP.NET Bundling and Minification](/guides/weboptimizer.html) or
[Cassette](/guides/cassette.html).