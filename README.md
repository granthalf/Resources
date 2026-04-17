```
####################################################################################
#
#                                 RESOURCES
#
####################################################################################

                                      SUMMARY

1. Directory {PYTHON}
  a) Pictures
      All resources to create ico/logos for building python programs.
      These pictures are mainly from Pixabay.


2. Directory {SCRIPTS}
  a) Browsers Extensions
      All resources to add Extensions to your Browser.





####################################################################################
#
#                                 TIPS
#
####################################################################################


A- WINDOWS 11
  1) Round Corner
      Microsoft decides for us what we need to use for computers. It's scandalous. It's not intuitive GUI. As example: Word. For OS, it has been decide round corners.
      What a bad idea! And if we don't accept and don't want, MIcrosoft not allow us! As dictatorship, they decide. We don't buy a product, we become slave of it.
      At least, we can use some product to retreive square corners: as ExplorerPatch (https://github.com/valinet/ExplorerPatcher).
      It has been worked then not work, another way was this tiny patch (https://github.com/valinet/Win11DisableRoundedCorners/releases).

  2) Firefox issue (text black on black)
      At least, I found an issue with a bad text on a bad back. I try the Dark Mode but nothing was nice.
      In order to find a solution, try to use by 'Help' then the 'Restart Firefox in Troubleshoot Mode'. It has been solved my issue, in my case
      (or not: troubleshoot is as a method "uninstall/install", so be careful with it ==> my case had for root cause one of my Scripts in "Monkey extension" & it was needed a debug process)

  3) Files Blocked!
      What a suppa Joy to find this point! Very Thanks Microsoft, to add sooooo many issues and generate a sooo big waste of time!
      Use Powershell and unlock your files, sometimes, to avoid this mechanism sooooo crazy:
      Get-ChildItem "C:\" -Recurse | Unblock-File
      Only One? Ok, only this: Unblock-File -Path "C:\<your_path>\file.ext"

  4) Root on Linux
      Basis but we can forget. Try this command to switch root.
      sudo -i

  5) Firefox Horizontal Scrollbar
      about:config
      widget.windows.overlay-scrollbars.enabled
      => switch to "false" (false => activate scrollbar)
      (+) go to settings, then check the checkbox: "Always show scrollbars"

  6) Raspberry
      a) Panel can't be edited (to add a lock button, for example)
      b) If you want to lock, you can by: Ctrl+Alt+L (https://forums.linuxmint.com, topic 22599)
      c) Create a Desktop Button
            create app.desktop on desktop
            with your favorite editor fill the file with the data below
            check your file explorer (as PcManFM) and check something like Edit / Prefs / check the box "don't ask any option for executable files"
### FILE ###
[Desktop Entry]
Type=Application
Name=<Name>
GenericName=<Name>
Comment=<desc>
Categories=System;Security;
Icon=/usr/img/<picture>.png
Exec=<here set your code as in a terminal>
Terminal=false
StartupNotify=false

  7) REMMINA
      Same as "wayland" and issues with keyboards other than us: but for this client, go on "Prefs" / "Use client keyboard mapping" (src= https://askubuntu.com/questions/586964/wrong-keyboard-layout-in-remmina-and-windows-server)

  8) ROUTE TO HOST: FAILED (FFPLAY)
      add to /etc/sysctl.conf with root:
      echo "net.ipv6.conf.all.disable_ipv6=1" >> /etc/sysctl.conf
      echo "net.ipv6.conf.default.disable_ipv6=1" >> /etc/sysctl.conf
      src= https://unix.stackexchange.com/questions/475257/getting-frequently-connection-error-no-route-to-host-and-tls-session-handshake

  9) PYTHON (Localhost)
      py -m http.server
      python -m http.server
      
      URL= http://127.0.0.1:8000/
      URL= http://localhost:8000/

  10) Unix - Keyboards & Lang (for session)
      [ALPINE] setup-keymap fr fr




####################################################################################
#
#                                 EXTERNAL LINKS
#
####################################################################################


[CYBERSECURITY]
{SEC LISTS} https://github.com/danielmiessler/SecLists
{NIS2} (fr) https://www.maire-info.com/cybermalveillance/cybersecurite-et-directive-nis-2-o%EF%BF%BD-en-est-on--article-30090


[ AD ]
{AD FOREST} (fr) https://www.varonis.com/fr/blog/foret-active-directory

[ UAC ]
{DEFINE} (fr) https://www.toutwindows.com/controle-de-compte-utilisateur-uac/

[ PASSWORDS ]
{DOCUMENTARY} (eng) [https://www.toutwindows.com/controle-de-compte-utilisateur-uac/](https://www.youtube.com/watch?v=m-OjoQBHPyU)

[ LINUX ]
{ONLINE SYSTEMS} (wana try one?) https://distrosea.com/



####################################################################################
#
#                                 MY PHILOSOPHY
#
####################################################################################


I'm someone who uses facts in first. Then, I have my own opinions.
All work shared is made with "a rule". A rule is applied for anyone.
If cookie are annoying me, I'm not alone versus cookies. It's a global issue.
Companies defend themselves to protect their commercial purposes.
But I defend myself on my own informations: I want do choices if all elements have been brought to me correctly.


1. I want share tools as near as possible than tools who match with these criteria:
- open source
- free
- reusable
- without cookies
- without advs
- without permissions as reaching personnal informations

=> With this mind, I limit highly all "attack surface".


2. With laws & governements, it's time to avoid these countries:
- USA. For spying & collecting informations. Governement is able to force companies to forward sensitives informations. Direct laws make Gov as an executive requester (no protection against request). 
- Russia. For spying & collecting informations. Governement is able to force companies to forward sensitives informations. Direct laws make Gov as an executive requester (no protection against request). 
- China. For spying & collecting informations. Governement is able to force companies to forward sensitives informations. Some laws make Gov as a requester (they have access and no protection against request). 

=> I'm from Europa, so my scope is: Europa.


3. Open Source:
This point makes anyone to build the app making the freedom not depending of a governement scope.
GIMP is made from USA but the source is from "open source". It's possible to check & analyze to be sure the app is safe (even if on first view it seems coming from a distrusted country).





```
