# open-air-crypt
This is a proof of concept python library for open-air cryptography. The goal
is to present a library that could be used to do short-range, over-the-air
cryptography that could be used for authenticating to a device using a
different device that you own, such as a cell phone. 

## Constraints
For this library to be usable, it will have to meet a number of constraints:

* Communicate using widely-used audio hardware (normal speakers & microphones)
* Limited to short range, as to not authenticate to devices you are not using

## Relevant Audio Libraries/Packages
* [amodem](https://github.com/romanz/amodem) - audio cable python program
> This program can transmit a file between 2 computers, using a simple headset,
> allowing true air-gapped communication (via a speaker and a microphone), or an
> audio cable (for higher transmission speed).
* [GNU Radio](https://wiki.gnuradio.org/index.php/Main_Page) - uses RF hardware
> GNU Radio is a free & open-source software development toolkit that provides
> signal processing blocks to implement software radios. It can be used with
> readily-available low-cost external RF hardware to create software-defined
> radios, or without hardware in a simulation-like environment. It is widely
> used in hobbyist, academic and commercial environments to support both
> wireless communications research and real-world radio systems.
* [libquiet](https://github.com/quiet/quiet) - seems to be ultrasonic only
> This library uses liquid SDR to transmit data through sound. This makes it
> suitable for sending data across a 3.5mm headphone jack or via speaker and mic.
> Quiet can build standalone binaries for encoding/decoding data via .wav files
> or for streaming through your soundcard via PortAudio. It can also be built as
> a library to be consumed by other C programs.

## Relevant Crypto Libraries
* [PGPy](https://github.com/SecurityInnovation/PGPy/) - PGP for Python
