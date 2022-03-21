# :zap: Javascript Click Drag

* Wes Bos Youtube Tutorial: [JavaScript Interface Challenge: Click and Drag to Scroll - #JavaScript30 27/30](https://www.youtube.com/watch?v=C9EWifQ5xqA&index=27&list=PLu8EoSxDXHP6CGK4YVJhL_VWetA865GOH).
* **Note:** to open web links in a new window use: _ctrl+click on link_

![GitHub repo size](https://img.shields.io/github/repo-size/AndrewJBateman/javascript-click-drag?style=plastic)
![GitHub pull requests](https://img.shields.io/github/issues-pr/AndrewJBateman/javascript-click-drag?style=plastic)
![GitHub Repo stars](https://img.shields.io/github/stars/AndrewJBateman/javascript-click-drag?style=plastic)
![GitHub last commit](https://img.shields.io/github/last-commit/AndrewJBateman/javascript-click-drag?style=plastic)

## :page_facing_up: Table of contents

* [:zap: Javascript Click Drag](#zap-javascript-click-drag)
  * [:page_facing_up: Table of contents](#page_facing_up-table-of-contents)
  * [:books: General info](#books-general-info)
  * [:camera: Screenshots](#camera-screenshots)
  * [:signal_strength: Technologies](#signal_strength-technologies)
  * [:floppy_disk: Setup](#floppy_disk-setup)
  * [:computer: Code Examples](#computer-code-examples)
  * [:cool: Features](#cool-features)
  * [:clipboard: Status & To-Do List](#clipboard-status--to-do-list)
  * [:clap: Inspiration](#clap-inspiration)
  * [:file_folder: License](#file_folder-license)
  * [:envelope: Contact](#envelope-contact)

## :books: General info

* Tutorial Code to scroll horizontally using click and drag.

## :camera: Screenshots

![Example screenshot](./img/drag.png).

## :signal_strength: Technologies

* [Javascript v1.9 ECMA-262 ECMAScript 2018](http://www.ecma-international.org/publications/standards/Ecma-262.htm)

## :floppy_disk: Setup

* Open `index.html` in browser. If any code is changed the browser needs to be refreshed.

## :computer: Code Examples

* calculate slider scroll left value from cursor position

```javascript
slider.addEventListener('mousemove', (e) => {
  if (!isDown) return; //stop the function from running
  console.log(isDown);
  e.preventDefault(); // prevent selection of text etc inside area.
  const x = e.pageX - slider.offsetLeft;
  const scrollMultiple = 3; // scroll 3 pixels for each pixel moved by the mouse.
  const walk = (x - startX)*scrollMultiple;
  slider.scrollLeft = scrollLeft - walk;
  console.log('slider scrollleft', slider.scrollLeft); //max value 4207.2001953125
});
```

## :cool: Features

* Scroll speed can be changed.

## :clipboard: Status & To-Do List

* Status: Working
* To-Do: Nothing

## :clap: Inspiration

* Wes Bos Youtube Tutorial: [JavaScript Interface Challenge: Click and Drag to Scroll - #JavaScript30 27/30](https://www.youtube.com/watch?v=C9EWifQ5xqA&index=27&list=PLu8EoSxDXHP6CGK4YVJhL_VWetA865GOH).

## :file_folder: License

* This project is licensed under the terms of the MIT license.

## :envelope: Contact

* Repo created by [ABateman](https://github.com/AndrewJBateman), email: gomezbateman@yahoo.com
