# hyperdom-ckeditor

```bash
npm install hyperdom-ckeditor
```

expects to have `window.CKEDITOR` already defined.

# usage

```js
function render() {
  return h('div',
    h('h1', 'ckeditor'),
    h('textarea', {binding: [this, 'html']}),
    ckeditor({binding: [this, 'html']})
  );
}
```

# api

```js
var vdom = ckeditor(options);
```

* `options.binding` - the binding to the model
* `options.config` - [ckeditor config](http://docs.ckeditor.com/#!/api/CKEDITOR.config).
* `options.inline` - [inline ckeditor](http://docs.ckeditor.com/#!/guide/dev_inline).
* `options` - the rest of the options are passed to create the vdom element, so you can use `class` and `key` among other things.

## We're Hiring!
Featurist provides full stack, feature driven development teams. Want to join us? Check out [our career opportunities](https://www.featurist.co.uk/careers/).
