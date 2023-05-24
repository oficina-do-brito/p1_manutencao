# my favorite software for development environment

:paperclip: Some of the software, tools that I always have installed on my machine and that help solve everyday problems :package:

## Linux

- [ ] snap

  ### How to Enable Snap Packages on Linux Mint 21

  To enable snap packages on Linux Mint 21 system, you need to perform a few steps carefully:

  Step 1: In the first step, you are required to delete the nosnap.pref file from the system. It would be done by executing the following command in the terminal:

  ```
    sudo rm /etc/apt/preferences.d/nosnap.pref
  ```

  Step 2: After removing the file, update the system repository to upgrade all the packages with the help of the given command:

  ```
    sudo apt update
  ```

  Step 3: Now, install the snap daemon on Linux Mint 21 system to manage and handle snap packages. Execute the command mentioned below to get snap daemon:

  ```
    sudo apt install snapd
  ```

  Step 4: After the installation of snapd, start it using the given command:

  ```
    sudo systemctl start snapd
  ```

  Step 5: In the next command you would be able to enable snapd, so that in the boot time, it starts automatically on the system:

  ```
    sudo systemctl enable snapd
  ```

  Step 6: Run the following command to check the successful installation of Snap on Linux Mint 21 system:

  ```
    snap version
  ```

  **summary of steps**:

  ```
    sudo rm /etc/apt/preferences.d/nosnap.pref &&
    sudo apt update &&
    sudo apt install snapd -y &&
    sudo systemctl start snapd &&
    sudo systemctl enable snapd &&
    snap version
  ```

- [ ] figma-linux -

  ```
    sudo snap install figma-linux
  ```

- [ ] OBS-studio

  ```
    sudo snap install obs-studio
  ```

- [ ] Olive

  ```
    sudo add-apt-repository ppa:olive-editor/olive-editor
    sudo apt-get update
    sudo apt-get install olive-editor -y
  ```

- [ ] Visual Studio Code

  ```
    sudo snap install code --classic
  ```

- [ ] Discord

  ```
    sudo snap install discord
  ```

- [ ] dbeaver-ce

  ```
    sudo snap install dbeaver-ce
  ```

- [ ] draw.io

  ```
    sudo snap install drawio
  ```

- [ ] Docker

  [installation link](https://docs.docker.com/engine/install/ubuntu/)

- [ ] gpicker

  ```
    sudo apt-get install gpick
  ```

- [ ] gimp

  ```
    sudo snap install gimp
  ```
