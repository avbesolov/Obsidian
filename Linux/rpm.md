#### rpm - менеджер пакетов
(рекурсивный акроним RPM Package Manager — RPM — менеджер пакетов) — формат пакетов программного обеспечения, а также программа, созданная для управления этими пакетами, используемые в ряде Linux-дистрибутивов.

|Description|Syntax|
|---|---|
|Install package|rpm -i _rpm-file_|
|Install verbose with a progress bar|rpm -ivh _rpm-file_|
|Extra verbose installation|rpm -ivvh _rpm-file_|
|Uninstall|rpm -e _package-name_|
|Uninstall verbose|rpm -ev _package-name_|
|Uninstall with extra verbose|rpm -evv _package-name_|
|Upgrade|rpm -Uvh _rpm-file_|
|List installed packages|rpm -qa|
|List files in an rpm|rpm -qpl _rpm-file_|
|List files for an installed package|rpm -ql _package-name_|
|List documentation/man pages for package|rpm -qd _package-name_|
|_rpm-file_ — Replace with actual rpm file _package-name_ — Replace with actual package name|   |

https://churchill.ddns.me.uk/post/rpm-cheat-sheet/ - cheatsheet