# &lt;musical-note&gt;

A [Polymer](https://www.polymer-project.org) element for a musical note in treble clef.

![alt tag](https://raw.githubusercontent.com/pianosnake/polymer-musical-note/master/demo/demo.png)

## Usage

Install using [Bower](http://bower.io/)

```
bower install polymer-musical-note
```

In your HEAD tag link the musical-note element

```
<link rel="import" href="bower_components/musical-note/musical-note.html">
```

In your HTML create `<musical-note>` tags with a value attribute set to a note name and octave. Middle C would have a value of c4. Numeric values are also supported. With numeric values add a *flat* attribute if you prefer the note to be rendered using a flat instead of a sharp.

```
<musical-note value="c"></musical-note>
<musical-note value="c#5"></musical-note>
<musical-note value="eb5"></musical-note>
<musical-note value="56" flat></musical-note>
```
The <musical-note> tags can be referenced like any other HTML elements.

```html
<musical-note value="c" id="firstnote"></musical-note>
```

```javascript
var firstNote = document.getElementById("firstNote");
```
Change the value of an existing note using `setValue`. Sharps are used by default, but if the second parameter is set to *true*, the note will be drawn using a flat instead of a sharp.</p>

```javascript
firstNote.setValue(60, true);
```

## Demo
The included demo file can be viewed using [Polyserve](https://github.com/PolymerLabs/polyserve). Install Polyserve using npm.

```
npm install polyserve -g
```
From the root of this project run polyserve

```
polyserve
```
Visit the demo page at [http://localhost:8080/components/musical-note/demo/](http://localhost:8080/components/musical-note/demo/)

## License

[MIT License](http://opensource.org/licenses/MIT)