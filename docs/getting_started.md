# Prerequisites

The first step is to install [Crystal](https://crystal-lang.org/) and it's system dependencies. Really all Crowsa needs is just the system's webview (and Crystal, since that's what Crowsa is bulit ontop of).

### Setting up for Linux

Install these system dependencies:

=== "Arch"

    ```sh
    pacman -Syu webkit2gtk crystal shards
    ```

=== "Ubuntu"

    ```sh
    apt update; sudo apt upgrade
    curl -fsSL https://crystal-lang.org/install.sh | bash
    ```

=== "Fedora"

    ```sh
    dnf update; sudo dnf upgrade
    dnf install webkitgtk crystal
    ```

=== "Gentoo"

    ```sh
    emerge --sync
    emerge -a dev-lang/crystal net-libs/webkit-gtk
    ```

=== "openSUSE"

    ```sh
    zypper refresh
    zypper install webkit2gtk crystal
    ```

=== "Void"

    ```sh
    xbps-install -S webkit2gtk crystal
    ```


That's it, you can now code your application via Crowsa

### Setting up for MacOS
Work in Progress

### Setting up for Windows

You need Microsoft Edge's [WebView2](https://developer.microsoft.com/en-us/microsoft-edge/webview2/?form=MA13LH#download) and Visual Studio.
Work in progress.
