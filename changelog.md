# 0.9.0
+ **Feature** [#64](https://github.com/VizuaaLOG/BulmaJS/issues/64) The alert plugin now has a `showHeader` option. This defaults to `true`, setting it to `false` will hide the alert's header.
+ **Feature** [#64](https://github.com/VizuaaLOG/BulmaJS/issues/64) The alert plugin now has `destroyOnConfirm` and `destroyOnCancel` options. These both default to `true` setting them to `false` will prevent the alert from destroying itself when the relevant button is clicked.
+ **Feature** [#64](https://github.com/VizuaaLOG/BulmaJS/issues/64) The alert plugin now has additional options for buttons. Supplying an object will allow you to also provide additional classes for each button. More details in the alert documentation.
+ **Tweak** [#65](https://github.com/VizuaaLOG/BulmaJS/issues/65) The alert callbacks now include an `event` argument. Thanks to [@alexcanana](https://github.com/alexcanana).
+ **Bug** Fixed a bug that caused `.modal` and `modal` classes to be applied to a modal

# 0.8.1
+ **Bug** [63](https://github.com/VizuaaLOG/BulmaJS/issues/63) Use a helper `each` method instead of `forEach`. This is to add support for IE11.

# 0.8.0
+ **Feature** [#47](https://github.com/VizuaaLOG/BulmaJS/issues/47) Implement an alert box. This extends the modal plugin and uses the card style. The type of alert box can be specified, adjusting the colours used.
+ **Tweak** [#61](https://github.com/VizuaaLOG/BulmaJS/pull/61) Remove the assumed window assignment, if you rely on this then you'll need to ensure you add this to you applications JS.
+ **Tweak BREAKING** The modal's `type` attribute has been renamed to `style`. This value is changing the 'style' of the modal, and so this better reflects the option.
+ **Bug** [#61](https://github.com/VizuaaLOG/BulmaJS/pull/61) Add a default export for the full BulmaJS bundle.
+ **Deprecated** Wikiki's Accordion plugin has been Deprecated from the core and will be removed in the 1.0 release. If you are using Wikiki's Accordion extension then it's recommended to use the official JS integration for it.
+ **Deprecated** Wikiki's Calendar plugin has been Deprecated from the core and will be removed from the 1.0 release. If you are using Wikiki's Calendar extension then it's recommended to use the official JS integration for it.

# 0.7.0
+ **Feature** [#27](https://github.com/VizuaaLOG/BulmaJS/issues/27) Modals can now be closed by pressing the 
`escape` key.
+ **Feature** [#27](https://github.com/VizuaaLOG/BulmaJS/issues/27) Modals can now be closed by clicking outside of an open modal.
+ **Feature** [#27](https://github.com/VizuaaLOG/BulmaJS/issues/27) When a modal is opening the `is-clipped` class is applied to the `body` element.
+ **Feature** Added a new `findElement` helper method to the BulmaJS core. This method will allow plugins to easily normalise an arugment that needs to be either an HTMLElement or a query selector string.
+ **Feature** [#27](https://github.com/VizuaaLOG/BulmaJS/issues/27) Rewrite the modal plugin, providing a new functionality, options and a full Javascript API.
+ **Feature** [#50](https://github.com/VizuaaLOG/BulmaJS/issues/50) Allow multiple plugins to be attached to a single class.
+ **Feature** [#39](https://github.com/VizuaaLOG/BulmaJS/issues/39) Implement a uniformed plugin interface
+ **Feature** [#40](https://github.com/VizuaaLOG/BulmaJS/issues/49) Add the ability for the navbar to be sticky at a certain threshold. Also add the ability for the navbar to hide on scroll down and reappear on scroll up. Thanks to [rdhar](https://github.com/rdhar) for the suggestion!
+ **Tweak** [#51](https://github.com/VizuaaLOG/BulmaJS/pull/51) Thanks to [apecell](https://github.com/apecell) the file plugin now supports drag and drop.
+ **Bug** [#27](https://github.com/VizuaaLOG/BulmaJS/issues/27) `closeButton` event is now correctly removed when destroying a modal.
+ **Bug** [#53](https://github.com/VizuaaLOG/BulmaJS/issues/53) The tabs plugin now ensures it only grabs the ul/li element that is a direct child of the `tabs-content` element.
+ **Bug** [#54](https://github.com/VizuaaLOG/BulmaJS/issues/54) Fix an issue where plugins were sometimes attached twice.

# 0.6.0
The reason for this being a large version jump is due to the complete overhaul of the documentation. While this doesn't change the functionality of the code, I feel like this is a large enough change to the project to warrant more than a 'patch' version bump.

+ [#36](https://github.com/VizuaaLOG/BulmaJS/issues/36) The navbar burger button now has the `is-active` class toggled.
+ [#22](https://github.com/VizuaaLOG/BulmaJS/issues/22) Documentation has had a redesign and a complete rewrite. If you find a typo please blame my keyboard ( :) ) and file an issue or submit a pull request.

# 0.5.0
+ [#38](https://github.com/VizuaaLOG/BulmaJS/pull/38) Adjust how plugins are initialised by using classes instead. Data attributes can still be used for customising the plugins behaviour, if supported. (closes [#20](https://github.com/VizuaaLOG/BulmaJS/issues/20))
+ [43b64cd](https://github.com/VizuaaLOG/BulmaJS/commit/43b64cdea58fe6b512ce95c69172889d75b68179) Add a new option to the tabs plugin that allows tabs to be changed when the user hovers over the tab link. On mobile this will revert back to the click/tap handler due to the lack of a hover event being called. (closes [#35](https://github.com/VizuaaLOG/BulmaJS/issues/35))

# 0.4.0
+ [#28](https://github.com/VizuaaLOG/BulmaJS/pull/28) Add the option to disable the modal being closable
+ [#31](https://github.com/VizuaaLOG/BulmaJS/pull/31) Add automated linting to the CI process (closes [#20](https://github.com/VizuaaLOG/BulmaJS/issues/29))

# 0.3.1
+ This changelog was added
+ Fix Wikiki's CSS files not being loaded on the docs
+ Publish to NPM
