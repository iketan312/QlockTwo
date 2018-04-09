WlockOne
========
In this repository you find the software, firmware and hardware design for the
"WlockOne", an open-source remake of the QLOCKTWO by BIEGERT & FUNK.

It is built by five I2IT under-grads computer science students.

Software
--------
The QlockToo Software Suite is written in PySide.

<img src="faceplate/face_21jul_reference_image.png" alt="faceplate">

Firmware
--------
We use an Arduino Micro as the central microcontroller.

License
-------
MIT-License - please refer to the License.txt in this repository.

Api
---
    @(get|set)brightness
        min                     int 0 - 255
        max                     int 0 - 255

    @(get|set)_nightmode
        brightness               int 0 - 255
        hour_start               int 0 - 23
        hour_end                 int 0 - 23
        minute_start             int 0 - 59
        minute_end               int 0 - 59

    @(get|set)kioskmode
        duration_words          int, minutes
        duration_seconds        int, minutes
        duration_temperature    int, minutes

    # matrix stream
    @m
        row     int 0 - 10
        values  bytearray

Errors
------

    !001 Unknown Command
    !002 Incorrect parameters

Authors
-------
- Ketan Ingale
