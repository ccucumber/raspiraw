raspiraw-modified
========

Two programs:
In C: ``raspi_dng``

and

in Python: ``mipi_raw10_to_jpg.py``


Prerequisites
=============

C compiler, Internet connection to download the required version of libtiff and a patch.

Build instructions
==================

Run ``make``, you will need a working Internet connection on the first run.


Usage
=====

* Transfer the output file to where you have ``raspi_dng``
* Convert to Adobe DNG:

        ./raspi_dng out.raw out.dng
     
* Or use Python:

        mipi_raw10_to_jpg.py out.raw out.jpg 4656 3496 bayer_rg
        mipi_raw10_to_jpg.py out.raw out.tiff 4656 3496 bayer_rg
     

See also
========

* Raspberry Pi forum topic: http://www.raspberrypi.org/phpBB3/viewtopic.php?t=44918&p=356676
* Sample Raspberry Pi JPEG+RAW images: http://bealecorner.org/best/RPi/
* dcraw homepage: http://www.cybercom.net/~dcoffin/dcraw/
