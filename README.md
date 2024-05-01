# B4B01NUM
CTU FEE Subject Numerical Analysis

- website: <https://cmp.felk.cvut.cz/~navara/nm/>
- moodle: <https://moodle.fel.cvut.cz/course/view.php?id=8195>
- remote connection via samba: `smb://aspace.msad.fel.cvut.cz/Data/Vyuka/NUM`

**Note:**\
.mw files are worksheets from Maple2023, for guaranteed compatibility it is recommended to use the same version of Maple.

## Maple Installation Guide
Instruction on how to install Maple2023 on Arch-based distributions.

Prerequisites: AUR helper (optional; `paru` is used in this tutorial), sudo privileges

1. Download software https://www.maplesoft.com/downloads/SelectPlatform.aspx?hash=07E8AECF22577B1F0F33697467FC2911.
    - Select Linux version, download will start automatically
    - If needed, license code is available on the official CTU website here: https://download.cvut.cz/maple-2023-for-students/
2. In the meantime, try to install [Maple2023](https://aur.archlinux.org/packages/maple2023) package from AUR . For `paru` AUR helper: `paru -S maple2023`. Installation will fail, but it will create a directory where we can move the `.run` file to make it work.
3. When the download is complete, move the `.run` file to the appropriate AUR helper cache directory. For `paru` it is located in 
    ```
    ~/.cache/paru/clone/maple2023/
    ```
4. Add executable privileges to the `.run` file using `chmod +x <installer_name>.run` command.
5. Now install [Maple2023](https://aur.archlinux.org/packages/maple2023) from AUR again. It will now find the crucial `.run` file and installation will continue. This takes several minutes and there is no debug info printed.
6. After a successful installation, you will be prompted in the terminal to activate your copy. Go to the mentioned directory 
    ```
    cd /usr/share/maple2023/bin
    ```
    and run the activation script with sudo privileges `sudo ./activation`.
    - Enter license code from the [CTU licenses website](https://download.cvut.cz/maple-2023-for-students/), your full name and your university email <nickname>@cvut.cz. This won't work with @fel.cvut.cz domain.
7. Installation process is complete. Maple should work now.


## License
GNU General Public License v3.0\
©2023 knedl1k
