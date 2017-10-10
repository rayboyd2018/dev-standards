# HTML standards
The following standards outline the requirements for production of HTML as served to end users. Any environment specific advice will be noted.

## DOCTYPE
Where practical, the doctype **must** be set to that of HTML5.

```
<!DOCTYPE html>
```

All documents should at minimum contain a `title`, `meta` tag dictating the character set, and the core structural elements, `html`, `head`, and `body`.

## Semantics
If possible, semantic HTML5 **should** be employed. This includes but is not limited to the use of `header`, `footer`, `nav`, `aside`, `section`, and `article` tags to denote semantically significant areas of a document.

The use of semantic HTML5 also eliminates the necessity of `role` attributes[1] in many cases and should be checked on a case-by-case basis.

### Using ARIA roles
Where possible, the native semantics of an HTML element should be adhered to. ARIA role attributes **must not** be used to redefine the semantics of any element, and **must** only be used to enhance otherwise undefined semantic value[2].

ARIA defined controls **must** be accessible by keyboard as well as a pointing device. This includes, but is not limited to controls such as dragging and dropping, sliding, and clicking on elements within a page.

Elements that should be legible by assistive devices or by standard screens **must not** contain an ARIA-based hiding mechanism such as `role="presentation"` or `aria-hidden="true"`.

## Validation
Where practical, internally maintained HTML must be validated via the standard HTML5 validator provided by W3[3]. This check will be performed as part of the standard QA process, but it is expected that a project be periodically checked for validity throughout development.

## Outline


## Responsive

[TBD - viewport meta, no disabling resize or zoom]

* [1] http://w3c.github.io/html/dom.html#wai-aria
* [2] https://w3c.github.io/using-aria/#rule1
