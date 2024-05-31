#poetryphone

A simple Asterisk configuration to play poetry sound files.

- Install Ubuntu 24.04
- apt-get install unzip git sox gnupg2 curl libnewt-dev libssl-dev libncurses5-dev subversion libsqlite3-dev build-essential libjansson-dev libxml2-dev libedit-dev uuid-dev subversion asterisk  asterisk-config asterisk-core-sounds-en asterisk-espeak asterisk-mp3 asterisk-moh-opsound-g722 asterisk-moh-opsound-gsm asterisk-core-sounds-en-g722

- adjust extensions.conf, pjsip.conf, pjsip_wizard.conf, sip.conf (see in this repo) and copy to /etc/asterisk

- copy audio files to /usr/local/share/asterisk/sounds

see the "Playback" lines in externsions.conf for the required file. The file name is usually the last name of the poet. if the Playback lines is

```Playback(lastname)````

a lastname.mp3 or lastname.gsm file is expected in /usr/local/share/asterisk/sounds

You can find audio files of poems at https://librivox.org/

