scroll-dom
==========

- Version: 0.0.1
- Technologies:
  - JavaScript
- Compatibility:
  - Chrome 45+
  - Firefox 36+
  - Internet Explorer 10+ (?)
  - Opera 35+
- Dependencies:
  - Development (optional):
    - utestjs (0.0.1)
- Copyright / Authors:
  - Krystian Pietruszka <kpietru@lokolab.net>
- Licenses:
  - MIT <http://opensource.org/licenses/MIT>
- Download: <https://github.com/lokolab/scroll-dom/releases>
- Homepage: <http://www.lokolab.net>

Scroll-dom is a JavaScript plugin for Luen library.
___________________________________________________

Example usage
-------------

    (function($) {
        $(document).ready(function() {
            $(document).scrollDom({
                callbackOneDown: function() {
                    $('#some-element').setPropertyStyle('color', 'green');
                },
                callbackOneUp: function() {
                    $('#some-element').setPropertyStyle('color', 'red');
                }
            });
        });
    })(luen);

API
---

- scrollDom ( object: __options__ ): self

References
----------

1. [Can one use Window. Onscroll method to include detection of scroll direction?][1]

[1]: http://stackoverflow.com/a/1223463
