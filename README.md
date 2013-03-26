## jQuery.base64 plugin ##

**jQuery.base64** is a jQuery plugin supports

- base64 codec function
- ajax integrated base64 decoding functionality

### Sample ###


```javascript
// encode/decode
$('#enc').html($.base64.encode(text))
$('#dec').html($.base64.decode($.base64.encode(text)))

// ajax integrated decoding
$.get('test2.txt', function(data){
    // variable data is already decoded to plain text
    $('#target').html(data)
}, 'text:b64')

$.get('test.html.txt', function(data){
    $('#target').html(data)
}, 'html:b64')
```

### Dependencies ###

Nothing without jQuery
