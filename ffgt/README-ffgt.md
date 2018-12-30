wusel@ysabell:/data/wusel$ git clone https://github.com/freifunk-gluon/gluon.git gluon-ffgt-v2018.2
wusel@ysabell:/data/wusel$ cd gluon-ffgt-v2018.2
wusel@ysabell:/data/wusel/gluon-ffgt-v2018.2$ git remote rename origin upstream
wusel@ysabell:/data/wusel/gluon-ffgt-v2018.2$ git remote add origin git@github.com:ffgtso/gluon-ffgt-v2018.2.git
wusel@ysabell:/data/wusel/gluon-ffgt-v2018.2$ git push -u origin master
wusel@ysabell:/data/wusel/gluon-ffgt-v2018.2$ git checkout v2018.2
wusel@ysabell:/data/wusel/gluon-ffgt-v2018.2$ git branch v2018.2-ffgt
wusel@ysabell:/data/wusel/gluon-ffgt-v2018.2$ git checkout v2018.2-ffgt
wusel@ysabell:/data/wusel/gluon-ffgt-v2018.2$ git push

wusel@ysabell:/data/wusel/gluon-ffgt-v2018.2$ patch --dry-run --verbose -p0 <ffgt/gluon_v2018.2-ffgt.diff 
Hmm...  Looks like a unified diff to me...
The text leading up to this was:
--------------------------
|--- package/gluon-respondd/src/respondd.c      2018-08-08 23:52:17.273286443 +0200
|+++ package/gluon-respondd/src/respondd.c      2018-08-10 04:20:15.427132029 +0200
--------------------------
checking file package/gluon-respondd/src/respondd.c
Using Plan A...
Hunk #1 succeeded at 127.
Hmm...  The next patch looks like a unified diff to me...
The text leading up to this was:
--------------------------
|--- package/gluon-web-admin/i18n/de.po 2018-08-08 23:53:06.718064404 +0200
|+++ package/gluon-web-admin/i18n/de.po 2018-08-10 04:20:15.431132092 +0200
--------------------------
checking file package/gluon-web-admin/i18n/de.po
Using Plan A...
Hunk #1 succeeded at 21.
Hunk #2 succeeded at 128 (offset 3 lines).
Hmm...  The next patch looks like a unified diff to me...
The text leading up to this was:
--------------------------
|--- package/gluon-status-page/files/lib/gluon/status-page/view/status-page.html        2018-08-08 23:53:06.718064404 +0200
|+++ package/gluon-status-page/files/lib/gluon/status-page/view/status-page.html        2018-12-21 04:51:30.733896561 +0100
--------------------------
checking file package/gluon-status-page/files/lib/gluon/status-page/view/status-page.html
Using Plan A...
Hunk #1 succeeded at 101 with fuzz 2.
Hmm...  The next patch looks like a unified diff to me...
The text leading up to this was:
--------------------------
|--- package/gluon-setup-mode/files/lib/gluon/setup-mode/rc.d/S20network        2018-08-08 23:52:17.273286443 +0200
|+++ package/gluon-setup-mode/files/lib/gluon/setup-mode/rc.d/S20network        2018-08-10 04:20:15.427132029 +0200
--------------------------
checking file package/gluon-setup-mode/files/lib/gluon/setup-mode/rc.d/S20network
Using Plan A...
Hunk #1 succeeded at 1.
Hunk #2 succeeded at 24.
Hmm...  The next patch looks like a unified diff to me...
The text leading up to this was:
--------------------------
|--- package/gluon-setup-mode/luasrc/lib/gluon/upgrade/320-setup-ifname 2018-08-08 23:52:17.273286443 +0200
|+++ package/gluon-setup-mode/luasrc/lib/gluon/upgrade/320-setup-ifname 2018-08-10 04:20:15.427132029 +0200
--------------------------
checking file package/gluon-setup-mode/luasrc/lib/gluon/upgrade/320-setup-ifname
Using Plan A...
Hunk #1 succeeded at 4.
Hmm...  The next patch looks like a unified diff to me...
The text leading up to this was:
--------------------------
|--- package/gluon-setup-mode/Makefile  2018-08-08 23:52:17.273286443 +0200
|+++ package/gluon-setup-mode/Makefile  2018-08-10 04:20:15.427132029 +0200
--------------------------
checking file package/gluon-setup-mode/Makefile
Using Plan A...
Hunk #1 succeeded at 9.
done
wusel@ysabell:/data/wusel/gluon-ffgt-v2018.2$ patch --verbose -p0 <ffgt/gluon_v2018.2-ffgt.diff
[…]
