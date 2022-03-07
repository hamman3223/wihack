## Diagram for Encryption
<br />
<p align="center">
    <img alt="WEP encapsulation block diagram" src="https://github.com/YWxtYXoK/wihack/blob/main/resources/wep_encapsulation.png" />
</p>

- <b>CRC-32 (Cyclic Redundancy Check)</b> - checksum algorithm used to detect corruption
- <b>RC4</b> - stream cipher
- <b>PRNG</b> - Pseudo Random Number Generator

<br />
<br />

## WEP Internals
<br />
<p align="center">
    <img alt="WEP MPDU" src="https://github.com/YWxtYXoK/wihack/blob/main/resources/wep_mpdu.png" />
</p>
- <a href="https://en.wikipedia.org/wiki/Frame_aggregation"><b>MPDU</b></a> - MAC protocol data unit

<br />
<br />

## WEP Decryption depends on IV
<br />
<p align="center">
    <img alt="WEP Decryption" src="https://github.com/YWxtYXoK/wihack/blob/main/resources/wep_decryption.png" />
</p>