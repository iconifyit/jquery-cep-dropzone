# jquery-cep-dropzone
A jQuery plugin to dynamically add a drop zone (drag-n-drop) for Adobe Illustrator CEP panels.

## Installation

```
<script src="https://code.jquery.com/jquery-3.4.1.min.js"></script>
<script src="/path/to/js/jquery-cep-dropzon.js"></script>
```
## Usage

```
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
