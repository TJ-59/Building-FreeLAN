# Building-FreeLAN
A guide to compiling a full static x64 version of FreeLAN for Windows and the required libraries, including a few fixes.

This github repository contains a guide for average Windows users wishing to compile the various libraries
needed for FreeLAN; and link, build and even package a slightly updated version of FreeLAN.

FreeLAN is "_A peer-to-peer, secure, easy-to-setup, multi-platform, open-source, highly-configurable VPN software_"
created by [Julien Kauffmann](https://github.com/ereOn), helped by many contributors over at [The freelan developers organization](https://github.com/freelan-developers).

The original FreeLAN repository is available [here](https://github.com/freelan-developers/freelan).

To use this guide, you'll need a few tools like NASM, Perl, Python, and some MSBuild tools
(Microsoft Visual Studio 2019/2022, or just the BuildTools 2019/2022).

FreeLAN requires a few open-source libraries :
ZLib, Miniupnpc, OpenSSL(v1.1.1+), Curl, Libiconv and Boost.

If you wish to make an installer out of it, you'll also need Inno Setup 6 and SCons.

All links to these ressources and setup hints are provided in the guide.

The modified files to be included are provided in a compressed archive, but for some of them you may simply modify the original files yourself.
The various MSBuild compatible files, mostly .vcxproj files, have been edited (for the x64 Release build only) to use relative paths for the various 
includes and required libraries, leaving only minor editing to do, in case of newer version of Boost.

Maintained by TJ-59


# Building-FreeLAN
Un guide pour compiler une version x64 entièrement statique de FreeLAN sous Windows et des librairies requises, qui inclut quelques correctifs.

Ce dépôt github contient un guide destiné aux utilisateurs moyens de Windows désirant compiler les multiples librairies nécessaires à FreeLAN,
et linker, construire et même faire un installeur d'une version légèrement améliorée de FreeLAN.

FreeLAN est un logiciel libre de réseau privé virtuel pair-à-pair, sécurisé, facile à mettre en place, multi-plateforme et hautement configurable,
créé par [Julien Kauffmann](https://github.com/ereOn), aidé par de nombreux contributeurs chez [The freelan developers organization](https://github.com/freelan-developers).

Le dépôt original de FreeLAN est disponible [ici](https://github.com/freelan-developers/freelan).

Pour utiliser ce guide, il vous faudra quelques outils tels que NASM, Perl, Python, et des outils MSBuild
(Microsoft Visual Studio 2019/2022, ou simplement les BuildTools 2019/2022).

FreeLAN nécessite quelques librairies open-source :
ZLib, Miniupnpc, OpenSSL(v1.1.1+), Curl, Libiconv et Boost.

Si vous souhaitez en faire un installeur, il vous faudra également Inno Setup 6 et SCons.

Tous les liens vers ces ressources et leurs conseils d'installation sont fournis dans le guide.

Les fichiers modifiés à inclure sont fournis dans une archive compressée, mais pour certains d'entre eux vous pouvez simplement les modifier vous-même.
Les fichiers compatibles MSBuild, principalement des .vcxproj, ont été édités (pour le build Release x64 uniquement) afin d'utiliser des chemins relatifs
pour les nombreux includes et librairies, ne laissant que des modifications mineures à faire, en cas de nouvelle version de Boost.

Entretenu par TJ-59
