#Updating pdfmake

To update to the newest pdfmake library checkout the new code, build the new code and copy over the files. Concatenate the two files to a single bundle.js file.

Project: https://github.com/bpampuch/pdfmake

Build the it from sources:

    git clone https://github.com/bpampuch/pdfmake.git
    cd pdfmake
    npm install # or: yarn
    git submodule update --init  libs/FileSaver.js
    npm run build # or: yarn run build

Cancatenate build/pdfmake.min.js and build/vfs_fonts.js (in this order) to the single file bundle.js

#Usage

Install via yarn (npm): 
    
    yarn add https://github.com/EcoLogicAG/pdfmake-browserify.git

Use with Angular CLI

    var pdfMake = require('pdfmake-browserify');

    ...

    pdfMake.createPDF(...)

    