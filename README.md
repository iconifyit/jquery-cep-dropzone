# jquery-cep-dropzone
A jQuery plugin to dynamically add a drop zone (drag-n-drop) for Adobe Illustrator CEP panels.

## Installation

```html
<script src="https://code.jquery.com/jquery-3.4.1.min.js"></script>
<script src="/path/to/js/jquery-cep-dropzon.js"></script>
```
## Usage

```javascript
$(function() {
    $('.cep-dropzone').cepDropZone({
        onSuccess : function(event, svg) {
            console.log('CEP Drag-n-Drop finished successfully (custom)', svg);
        },
        onError : function(event, error) {
            console.error('Oops! CEP Drag-n-Drop encountered an error. (custom)');
        }
    });
})
```

## Styling the dropzone

The default CSS for the DropZone is inserted into the HTML `<head/>` via JS so that the entire plugin is self-contained in a single file. No external CSS file to link.

You can over-ride these styles with :

```css
.dropozone {
    /* Your rules here */
}

.dropzone:hover {
    /* Your rules here */
}
```

That's it. Just two simple style selectors.
