# Scripts #

dump\_exif.py
> Output the EXIF file from a given file.
setgps.py
> Set GPS coordinates on a file.
getgps.py
> Get GPS coordinates from a file.
noop.py
> This is a no-op on a jpeg file. Useful for testing images are preserved across operations using pexif. Note that the binary data will not be exact as pexif will compress unused space in the file, however running it on a file twice should end up with the same data.