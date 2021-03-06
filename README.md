vue-picture-input
=============

Mobile-friendly picture file input Vue.js component with image preview, drag and drop, and EXIF orientation.

![Picture Input Demo](http://i.giphy.com/3o84UfcY1QV7Unrtba.gif)


## Installation

###npm

``` sh
npm install --save vue-picture-input
```

## Usage

```javascript
<script>
import PictureInput from 'vue-picture-input'

export default {
  name: 'app',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  },
  components: {
    PictureInput
  },
  methods: {
    onChange () {
      console.log("Picture changed!")
    }
  }
}
</script>
```

```HTML
<template>
  <div class="hello">    
    <picture-input @change="onChange()" width="600" height="600" margin="16" accept="image/jpeg,image/png"></picture-input>   
  </div>
</template>
```

## Props

- **width, height**: (pixels, optional) the width and the height of the preview container. The picture will be resized and centered to cover this area. If not specified, the preview container will expand to full width, 1:1 square ratio.
- **margin**: (pixels, optional) the margin around the preview container.
- **accept**: (media type, optional) the accepted image type(s) (e.g. image/jpeg, image/gif, etc.) Default value: image/*. 
- **id, name**: (string, optional) the id and name attributes of the HTML input element.

## Events

- **change**: emitted on (successful) picture change.


## TODOs

- Add support for multiple files 
- Demo GitHub pages


## Contributions

All contributions are welcome.
