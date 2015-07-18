# js-barcode
Pure JavaScript implementation of barcodes

Currently, only Code 39 is supported.

Use the barcode-code39.js in your html and use the GenerateCode39 function to get the barcode.

Docs for GenerateCode39:

    GenerateCode39 : Generate a code 39 barcode
    Inputs:
        data : Should be something that is representable as a string. 
               Code 39 is limited and big, so don't make the data argument too long.
        useCanvas : true  = Draw the code 39 barcode in a 2d canvas context.
                    false = Return a dynamically created div containing synamically created spans
                            representing the barcode.
                    Default: true
        returnImg : true =  Convert the canvas into a data URL and 
                            make that the src of a dynamically created img element.
                            Return the dynamically created img element.
                    false = Return the dynamically created canvas element.
                    Default: true if useCanvas == true, else false
        settings : object
                   {
                     widtBarWidth     : positive integer pixels  (default = 4)
                     narrowBarWidth   : positive integer pixels  (default = 2)
                     wideSpaceWidth   : positive integer pixels  (default = 4)
                     narrowSpaceWidth : positive integer pixels  (default = 2)
                     barcodeHeight    : positive integer pixels  (default = 36)
                   }
    Outputs:
        canvas element or img element or div element on success based on inputs
        null on no data

Released under the GNU GPLv2 license and with no warranty.

Enjoy!

