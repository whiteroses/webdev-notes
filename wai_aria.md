# WAI-ARIA

Web Accessibility Initiative Accessible Rich Internet Applications (Suite?)

Defines a way to make web content and applications more accessible to people
with disabilities.


## Links

* [WAI-ARIA Authoring Practices 1.1](https://www.w3.org/TR/wai-aria-practices/)
* [ARIA in HTML](https://www.w3.org/TR/html-aria/)
* https://www.w3.org/WAI/intro/aria


## Landmark regions

### Default landmark roles for HTML5 sectioning elements

HTML5 Element | Default Landmark Role
--------------|----------------------
`aside`       | `complementary`
`footer`      | `contentinfo` when in context of the `body` element
`header`      | `banner` when in context of the `body` element
`main`        | `main`
`nav`         | `navigation`
`section`     | `region` when it has an accessible name using `aria-labelledby` or `aria-label`
