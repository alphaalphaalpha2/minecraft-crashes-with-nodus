minecraft-crashes-with-nodus
============================

can someone help me with this crash! nodus crashes when clicking resource packs ---- Minecraft Crash Report ---- // Why is it breaking :(  Time: 11/8/14 2:33 PM Description: Updating screen events  java.lang.IllegalArgumentException: input == null! 	at javax.imageio.ImageIO.read(Unknown Source) 	at net.minecraft.client.resources.DefaultResourcePack.getPackImage(DefaultResourcePack.java:107) 	at net.minecraft.client.resources.ResourcePackListEntryDefault.&lt;init>(ResourcePackListEntryDefault.java:28) 	at net.minecraft.client.gui.GuiScreenResourcePacks.initGui(GuiScreenResourcePacks.java:70) 	at net.minecraft.client.gui.GuiScreen.setWorldAndResolution(GuiScreen.java:274) 	at net.minecraft.client.Minecraft.displayGuiScreen(Minecraft.java:832) 	at net.minecraft.client.gui.GuiOptions.actionPerformed(GuiOptions.java:136) 	at net.minecraft.client.gui.GuiScreen.mouseClicked(GuiScreen.java:244) 	at net.minecraft.client.gui.GuiScreen.handleMouseInput(GuiScreen.java:327) 	at net.minecraft.client.gui.GuiScreen.handleInput(GuiScreen.java:291) 	at net.minecraft.client.Minecraft.runTick(Minecraft.java:1703) 	at net.minecraft.client.Minecraft.runGameLoop(Minecraft.java:1016) 	at net.minecraft.client.Minecraft.run(Minecraft.java:931) 	at net.minecraft.client.main.Main.main(Main.java:109) 	at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method) 	at sun.reflect.NativeMethodAccessorImpl.invoke(Unknown Source) 	at sun.reflect.DelegatingMethodAccessorImpl.invoke(Unknown Source) 	at java.lang.reflect.Method.invoke(Unknown Source) 	at magic.launcher.Launcher.main(SourceFile:207)   A detailed walkthrough of the error, its code path and all known details is as follows: ---------------------------------------------------------------------------------------  -- Head -- Stacktrace: 	at javax.imageio.ImageIO.read(Unknown Source) 	at net.minecraft.client.resources.DefaultResourcePack.getPackImage(DefaultResourcePack.java:107) 	at net.minecraft.client.resources.ResourcePackListEntryDefault.&lt;init>(ResourcePackListEntryDefault.java:28) 	at net.minecraft.client.gui.GuiScreenResourcePacks.initGui(GuiScreenResourcePacks.java:70) 	at net.minecraft.client.gui.GuiScreen.setWorldAndResolution(GuiScreen.java:274) 	at net.minecraft.client.Minecraft.displayGuiScreen(Minecraft.java:832) 	at net.minecraft.client.gui.GuiOptions.actionPerformed(GuiOptions.java:136) 	at net.minecraft.client.gui.GuiScreen.mouseClicked(GuiScreen.java:244) 	at net.minecraft.client.gui.GuiScreen.handleMouseInput(GuiScreen.java:327) 	at net.minecraft.client.gui.GuiScreen.handleInput(GuiScreen.java:291)  -- Affected screen -- Details: 	Screen name: net.minecraft.client.gui.GuiScreenResourcePacks Stacktrace: 	at net.minecraft.client.Minecraft.runTick(Minecraft.java:1703) 	at net.minecraft.client.Minecraft.runGameLoop(Minecraft.java:1016) 	at net.minecraft.client.Minecraft.run(Minecraft.java:931) 	at net.minecraft.client.main.Main.main(Main.java:109) 	at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method) 	at sun.reflect.NativeMethodAccessorImpl.invoke(Unknown Source) 	at sun.reflect.DelegatingMethodAccessorImpl.invoke(Unknown Source) 	at java.lang.reflect.Method.invoke(Unknown Source) 	at magic.launcher.Launcher.main(SourceFile:207)  -- System Details -- Details: 	Minecraft Version: 1.7.2 	Operating System: Windows 8.1 (x86) version 6.3 	Java Version: 1.7.0_67, Oracle Corporation 	Java VM Version: Java HotSpot(TM) Client VM (mixed mode, sharing), Oracle Corporation 	Memory: 369612024 bytes (352 MB) / 518979584 bytes (494 MB) up to 518979584 bytes (494 MB) 	JVM Flags: 3 total; -Xms512m -Xmx512m -XX:HeapDumpPath=MojangTricksIntelDriversForPerformance_javaw.exe_minecraft.exe.heapdump 	AABB Pool Size: 0 (0 bytes; 0 MB) allocated, 0 (0 bytes; 0 MB) used 	IntCache: cache: 0, tcache: 0, allocated: 0, tallocated: 0 	Launched Version: Nodus 	LWJGL: 2.9.0 	OpenGL: Intel(R) HD Graphics GL version 4.0.0 - Build 10.18.10.3379, Intel 	Is Modded: Very likely; Jar signature invalidated 	Type: Client (map_client.txt) 	Resource Packs: [] 	Current Language: English (US) 	Profiler Position: N/A (disabled) 	Vec3 Pool Size: ~~ERROR~~ NullPointerException: null 	Anisotropic Filtering: Off (1)

here is a better version

---- Minecraft Crash Report ----
// Why is it breaking :(

Time: 11/8/14 2:33 PM
Description: Updating screen events

java.lang.IllegalArgumentException: input == null!
	at javax.imageio.ImageIO.read(Unknown Source)
	at net.minecraft.client.resources.DefaultResourcePack.getPackImage(DefaultResourcePack.java:107)
	at net.minecraft.client.resources.ResourcePackListEntryDefault.<init>(ResourcePackListEntryDefault.java:28)
	at net.minecraft.client.gui.GuiScreenResourcePacks.initGui(GuiScreenResourcePacks.java:70)
	at net.minecraft.client.gui.GuiScreen.setWorldAndResolution(GuiScreen.java:274)
	at net.minecraft.client.Minecraft.displayGuiScreen(Minecraft.java:832)
	at net.minecraft.client.gui.GuiOptions.actionPerformed(GuiOptions.java:136)
	at net.minecraft.client.gui.GuiScreen.mouseClicked(GuiScreen.java:244)
	at net.minecraft.client.gui.GuiScreen.handleMouseInput(GuiScreen.java:327)
	at net.minecraft.client.gui.GuiScreen.handleInput(GuiScreen.java:291)
	at net.minecraft.client.Minecraft.runTick(Minecraft.java:1703)
	at net.minecraft.client.Minecraft.runGameLoop(Minecraft.java:1016)
	at net.minecraft.client.Minecraft.run(Minecraft.java:931)
	at net.minecraft.client.main.Main.main(Main.java:109)
	at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method)
	at sun.reflect.NativeMethodAccessorImpl.invoke(Unknown Source)
	at sun.reflect.DelegatingMethodAccessorImpl.invoke(Unknown Source)
	at java.lang.reflect.Method.invoke(Unknown Source)
	at magic.launcher.Launcher.main(SourceFile:207)


A detailed walkthrough of the error, its code path and all known details is as follows:
---------------------------------------------------------------------------------------

-- Head --
Stacktrace:
	at javax.imageio.ImageIO.read(Unknown Source)
	at net.minecraft.client.resources.DefaultResourcePack.getPackImage(DefaultResourcePack.java:107)
	at net.minecraft.client.resources.ResourcePackListEntryDefault.<init>(ResourcePackListEntryDefault.java:28)
	at net.minecraft.client.gui.GuiScreenResourcePacks.initGui(GuiScreenResourcePacks.java:70)
	at net.minecraft.client.gui.GuiScreen.setWorldAndResolution(GuiScreen.java:274)
	at net.minecraft.client.Minecraft.displayGuiScreen(Minecraft.java:832)
	at net.minecraft.client.gui.GuiOptions.actionPerformed(GuiOptions.java:136)
	at net.minecraft.client.gui.GuiScreen.mouseClicked(GuiScreen.java:244)
	at net.minecraft.client.gui.GuiScreen.handleMouseInput(GuiScreen.java:327)
	at net.minecraft.client.gui.GuiScreen.handleInput(GuiScreen.java:291)

-- Affected screen --
Details:
	Screen name: net.minecraft.client.gui.GuiScreenResourcePacks
Stacktrace:
	at net.minecraft.client.Minecraft.runTick(Minecraft.java:1703)
	at net.minecraft.client.Minecraft.runGameLoop(Minecraft.java:1016)
	at net.minecraft.client.Minecraft.run(Minecraft.java:931)
	at net.minecraft.client.main.Main.main(Main.java:109)
	at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method)
	at sun.reflect.NativeMethodAccessorImpl.invoke(Unknown Source)
	at sun.reflect.DelegatingMethodAccessorImpl.invoke(Unknown Source)
	at java.lang.reflect.Method.invoke(Unknown Source)
	at magic.launcher.Launcher.main(SourceFile:207)

-- System Details --
Details:
	Minecraft Version: 1.7.2
	Operating System: Windows 8.1 (x86) version 6.3
	Java Version: 1.7.0_67, Oracle Corporation
	Java VM Version: Java HotSpot(TM) Client VM (mixed mode, sharing), Oracle Corporation
	Memory: 369612024 bytes (352 MB) / 518979584 bytes (494 MB) up to 518979584 bytes (494 MB)
	JVM Flags: 3 total; -Xms512m -Xmx512m -XX:HeapDumpPath=MojangTricksIntelDriversForPerformance_javaw.exe_minecraft.exe.heapdump
	AABB Pool Size: 0 (0 bytes; 0 MB) allocated, 0 (0 bytes; 0 MB) used
	IntCache: cache: 0, tcache: 0, allocated: 0, tallocated: 0
	Launched Version: Nodus
	LWJGL: 2.9.0
	OpenGL: Intel(R) HD Graphics GL version 4.0.0 - Build 10.18.10.3379, Intel
	Is Modded: Very likely; Jar signature invalidated
	Type: Client (map_client.txt)
	Resource Packs: []
	Current Language: English (US)
	Profiler Position: N/A (disabled)
	Vec3 Pool Size: ~~ERROR~~ NullPointerException: null
	Anisotropic Filtering: Off (1)
	
	help
