Find:

    timedatectl list-timezones | grep -i moscow

Europe/Moscow

Set:

    timedatectl set-timezone Europe/Moscow

View:

    timedatectl

For older version(w/o timedatectl)

    echo "Europe/Rome" | sudo tee /etc/timezone

    sudo dpkg-reconfigure --frontend noninteractive tzdata