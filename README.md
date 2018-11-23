#PDFMerger for PHP (PHP 5/Symfony Compatible) with TCPDF

Original written by http://pdfmerger.codeplex.com/team/view port to PHP 5 by https://github.com/myokyawhtun/PDFMerger

## Symfony Compatible

Based on https://github.com/rguedes/PDFMerger.
FPDF/FPDI replaced by TCPDF because of FPDI free version not able handle all PDF compressions type.

### Example Usage
```php

$pdf = new \PDFMerger;

$pdf->addPDF('samplepdfs/one.pdf', '1, 3, 4');
$pdf->addPDF('samplepdfs/two.pdf', '1-2');
$pdf->addPDF('samplepdfs/three.pdf', 'all');


$pdf->merge('file', 'samplepdfs/TEST2.pdf'); 
    
// REPLACE 'file' WITH 'browser', 'download', 'string', or 'file' for output options
```
