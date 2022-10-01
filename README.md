# PDF Into JPG
Exports images inTO JPG from a PDF file to disk.

## Use via CLI
```
Usage: npx pdf-into-jpg <file> [dir]

Arguments:
  file        path to PDF file
  dir         image destination directory (default: ".")
```
You can also install the package globally via `npm i -g pdf-into-jpg` to run the command without `npx`

## Programatic use
install
```sh
npm i pdf-into-jpg
```

`script.js`
```js
import { exportImages } from 'pdf-into-jpg'
exportImages('file.pdf', 'output/dir')
  .then(images => console.log('Exported', images.length, 'images'))
  .catch(console.error)
```

See: [cli.js](https://github.com/Tibex88/pdf-into-jpg/blob/main/cli.js#L23) for progress details during export.