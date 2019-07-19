# Image-Uploader
Image-Uploader is a simple jQuery Drag & Drop Image Uploader plugin made to be used in forms, withot AJAX.

## Demo
[Demo page here](https://christianbayer.github.io/image-uploader/)

## How to use it
Import the CSS file at the `<head>` along Material Icons for the icons:
```
<link type="text/css" rel="stylesheet" href="https://fonts.googleapis.com/icon?family=Material+Icons">
<link type="text/css" rel="stylesheet" href="http://example.com/image-uploader.min.css">
```
Import the JS file at the end of the `<body>`, after the jQuery:
```
<script type="text/javascript" src="http://example.com/jquery.min.js"></script>
<script type="text/javascript" src="http://example.com/image-uploader.js"></script>
```
Create a form with `enctype="multipart/form-data"` attributte:
```
<form action="http://example.com/post" enctype="multipart/form-data"></form>
```
Inside the form, create a wrapper to the plugin:
```
<div class="input-images"></div>
```
Initialize it with jQuery 
```
$('.input-images').imageUploader();
```

## Options

#### label
Type: `string`

Default: `'Drag & Drop files here or click to browse'`

Informative label, telling the user what to do with the draggable area.

#### preloaded
Type: `{id: number, src: string}[]`

Default: `[]`

Array of objects representing images that are already stored, containing an identification for that image and the source.

#### imagesInputName
Type: `string`

Default: `'images'`

Name of the input that will be posted, containing the files list.

#### preloaded
Type: `string`

Default: `'preloaded'`

Name of the inputs that will be posted, containing the preloaded images identification.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details