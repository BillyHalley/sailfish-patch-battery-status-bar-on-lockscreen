sailfishos-patch-voicecallui-keypad-by-default
==============================================

This simple patch (really, it's one line!) makes the Dialer Keypad open by default when opening the "Phone" application.  
That's it.

# NOTICE:
#
# Application name defined in TARGET has a corresponding QML filename.
# If name defined in TARGET is changed, the following needs to be done
# to match new name:
#   - corresponding QML filename must be changed
#   - desktop icon filename must be changed
#   - desktop filename must be changed
#   - icon definition filename in desktop file must be changed
#   - translation filenames have to be changed

# The name of your application
TARGET = battery-status-bar-on-lockscreen

TEMPLATE = aux

patch.path = /usr/share/patchmanager/patches/ziobilly-battery-status-bar-on-lockscreen
patch.files = data/unified_diff.patch data/patch.json

INSTALLS += \
	patch


OTHER_FILES += \
    rpm/sailfishos-patch-battery-status-bar-on-lockscreen.changes.in \
    data/patch.json \
    data/unified_diff.patch

