# iframe

Nested browsing context, effectively embedding another HTML page into current
page. Each browsing context has its own session history and active document.

Parent browsing context:: browsing context that contains the embedded content

The top-level browsing context (which has no parent) is typically the browser
window.


## Attributes

### name

Name for the embedded browsing context. This can be used as the value of the
`target` attribute of an `<a>` or `<form>` element, or the `formtarget`
attribute of an `<input>` or `<button>` element.

### sandbox

HTML5 only. Enables extra restrictions on the content that can appear in the
inline frame. The value of the attribute can either be an empty string (all the
restrictions are applied), or a space-separated list of tokens that life
particular restrictions. Not supported in IE 9 or earlier.
	
### src

### referrerpolicy

Experimental according to MDN?


## Scripting

Inline frames enter the `window.frames` pseudo-array.

From the DOM `iframe` element, scripts can get access to the `window` object of
the included HTML page via the `contentWindow` property. The `contentDocument`
property refers to the document element inside the iframe, equivalent to
`contentWindow.document`.

From the inside of a frame, a script can get a reference to the parent window
via `Window.parent`.

Scripts trying to access a frame's content, and scripts inside a frame trying
to access its parent window, are both subject to the same-origin policy.
Cross-domain communication can still be achieved with `Window.postMessage()`.
