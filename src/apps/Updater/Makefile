AUTOUPDATE_ICON = 'build_xcode/build/Release/Karabiner-Elements.app/Contents/Frameworks/Sparkle.framework/Versions/A/Resources/Autoupdate.app/Contents/Resources/AppIcon.icns'

all:
	make -C ../lib/KarabinerKit
	make build_xcode
	install -m 644 ../share/Resources/app.icns $(AUTOUPDATE_ICON)

clean: clean_builds

run:
	./build_xcode/build/Release/Karabiner-Elements.app/Contents/MacOS/Karabiner-Elements

run_stable:
	./build_xcode/build/Release/Karabiner-Elements.app/Contents/MacOS/Karabiner-Elements checkForUpdatesStableOnly

include ../../Makefile.rules
