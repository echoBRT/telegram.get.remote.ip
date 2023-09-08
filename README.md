Telegram get remote IP
New 2023 version written in python, against bash.

This script is intended to be used to determine the IP address of the interlocutor in the telegram messenger.

You must have tshark installed to use it.

Attention! To determine the IP address, you must be in each other's contacts.

Get caller IP
How to use?

    Install Telegram desktop client on Linux or Mac.
    Install tshark (sudo apt install tshark or download for macOS here, it's comes with wireshark).
    Run script, call and wait for an answer.
    Profit! You have received the IP address of the interlocutor.

Get & Run (Ubuntu 20 example)

$ sudo apt update
$ sudo apt install -y python3-pip python3-venv tshark
$ git clone https://github.com/n0a/telegram-get-remote-ip
$ cd telegram-get-remote-ip
$ python3 -m venv venv
$ source ./venv/bin/activate
$ sudo pip3 install -r requirements.txt
$ sudo python3 tg_get_ip.py

Or specify the interface immediately at startup:

$ sudo python3 -i en0 tg_get_ip.py

PS. Possible work with termux on android smartphones. Root authority is required to capture traffic.
