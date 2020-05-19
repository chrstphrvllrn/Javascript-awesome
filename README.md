# Javascript-awesome
### https://help.github.com/en/github/writing-on-github/basic-writing-and-formatting-syntax
## creating favicon

https://favicon.io/favicon-generator/

## icons

https://www.npmjs.com/package/font-awesome

## string manupulation

1. https://www.npmjs.com/package/strings-library 
   github: https://github.com/jshams/npm-libraries-few2-1/tree/master/strings-library
   ```javascript
   const str = 'i like yellow water baloons'
    str.firstCharToUpper()          // 'I like yellow water baloons'
    str.allCaps()                   // 'I LIKE YELLOW WATER BALOONS'
    str.upperEveryOtherLetter()     // 'I lIkE yElLoW wAtEr BaLoOnS'
    str.removeWhiteSpace()          // 'i like yellow water baloons'
    str.kabobCase()                 // 'i-like-yellow-water-baloons'
    str.snakeCase()                 // 'i_like_yellow_water_baloons'
    str.camelCase()                 // 'iLikeYellowWaterBaloons'
    ```
    
2. https://html-cleaner.com/case-converter/
   https://html-cleaner.com/case-converter/js/convertcase.js?y=2019
   
   
   
  ```javascript
   const str = 'i like yellow water baloons'
   sentenceCase(str)
   alternatingCase(str)
   randomCase(str)
   ucwords(str)
 
   ```



## File Info

1. https://www.npmjs.com/package/convert-size
   ```javascript
   const { default: convertSize } = require("convert-size");
   // or
   import convertSize from "convert-size";

   convertSize(1000); // => 1 KB
   convertSize(1000 * 1000); // => 1 MB
   convertSize("1 MB"); // => 1000000
   convertSize("1 GB", "MB"); // => 1000
   convertSize(1000000, "KB"); // => 1000
   convertSize("1 mb", "GB", { stringify: true }); // => 0.001 GB

   // to know more about option read the options part below
   convertSize(1000 * 1000, {
     accuracy: 0,
     shortcut: false
   }); // => 1 Kilo Byte
   
   
   ```
   
 2. https://stackoverflow.com/questions/15900485/correct-way-to-convert-size-in-bytes-to-kb-mb-gb-in-javascript
   
 
   ```javascript
   
   var num = '1000'
   var formatBytes = (bytes, decimals = 2) => {
      if (bytes === 0) return '0 Bytes';

      const k = 1024;
      const dm = decimals < 0 ? 0 : decimals;
      const sizes = ['Bytes', 'KB', 'MB', 'GB', 'TB', 'PB', 'EB', 'ZB', 'YB'];

      const i = Math.floor(Math.log(bytes) / Math.log(k));

      return parseFloat((bytes / Math.pow(k, i)).toFixed(dm)) + ' ' + sizes[i];
		}
      
      
        formatBytes(num)
   ```
   
   

# Uploading files

1. https://github.com/taniarascia/upload

2. https://web.dev/read-files/

3. https://github.com/justindn/fileupload

4. https://nielsboogaard.github.io/filepond-plugin-media-preview/
   https://github.com/pqina/filepond
   
5. https://github.com/blueimp/jQuery-File-Upload
   
# JQuery 

1. https://learn.jquery.com/using-jquery-core/selecting-elements/
