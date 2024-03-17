![Ransomlettter](https://github.com/MarcuXNg/Introduction_to_Cyber_Security_Writeup/assets/95072521/a26f95fa-5b8d-492e-be0d-62a6dbe73112)

- `sudo apt install poppler-utils` to install `pdfinfo`

![pdfinfo](https://github.com/MarcuXNg/Introduction_to_Cyber_Security_Writeup/assets/95072521/5b99d1d6-5099-4aa4-89ce-aa9babe60138)

[Answer] 
- the author of the attached pdf file: Ann Gree Shepherd

### Photo EXIF Data

- EXIF stands for Exchangeable Image File Format, a standard for saving metadata to image files
- metadata that can be found in the original digital images:
    + Camera model/ smartphone model
    + Date and time of the image capture
    + Photo settings (focal length, aperture, shutter speed, and ISO settings)
- Finding GPS coordinates embedded in the image is highly probable (smartphones are equipped with a GPS sensor)
- The GPS coordinates (latitude and longitude): generally show the place where the photo was taken.
- `exiftool`: use to read and write metadata in various file types, such as JPEG images. (`sudo apt install libimage-exiftool-perl` to install the exiftool) 
- Searching `Microsoft Bing Maps` or `Google Maps` for THECOORDINATES reveals that these coordinates indicate where the images was taken.

![exiftool](https://github.com/MarcuXNg/Introduction_to_Cyber_Security_Writeup/assets/95072521/ac5ddd9a-c3db-4207-916f-73d284907d24)