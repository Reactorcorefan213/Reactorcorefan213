- PLEASE HELP GUYS!!!!!!!!!!!!!  IT KEEPS CRASHING!!!!  java.lang.ClassNotFoundException: codechicken.multipart.BlockMultipart
HERES LOG:
---- Minecraft Crash Report ----
// You should try our sister game, Minceraft!

Time: 02/05/21 09:00
Description: There was a severe problem during mod loading that has caused the game to fail

cpw.mods.fml.common.LoaderException: java.lang.NoClassDefFoundError: codechicken/multipart/BlockMultipart
	at cpw.mods.fml.common.LoadController.transition(LoadController.java:163)
	at cpw.mods.fml.common.Loader.loadMods(Loader.java:544)
	at cpw.mods.fml.client.FMLClientHandler.beginMinecraftLoading(FMLClientHandler.java:208)
	at net.minecraft.client.Minecraft.func_71384_a(Minecraft.java:480)
	at net.minecraft.client.Minecraft.func_99999_d(Minecraft.java:878)
	at net.minecraft.client.main.Main.main(SourceFile:148)
	at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method)
	at sun.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:62)
	at sun.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43)
	at java.lang.reflect.Method.invoke(Method.java:497)
	at net.minecraft.launchwrapper.Launch.launch(Launch.java:135)
	at net.minecraft.launchwrapper.Launch.main(Launch.java:28)
Caused by: java.lang.NoClassDefFoundError: codechicken/multipart/BlockMultipart
	at java.lang.Class.forName0(Native Method)
	at java.lang.Class.forName(Class.java:348)
	at cpw.mods.fml.common.FMLModContainer.constructMod(FMLModContainer.java:440)
	at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method)
	at sun.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:62)
	at sun.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43)
	at java.lang.reflect.Method.invoke(Method.java:497)
	at com.google.common.eventbus.EventSubscriber.handleEvent(EventSubscriber.java:74)
	at com.google.common.eventbus.SynchronizedEventSubscriber.handleEvent(SynchronizedEventSubscriber.java:47)
	at com.google.common.eventbus.EventBus.dispatch(EventBus.java:322)
	at com.google.common.eventbus.EventBus.dispatchQueuedEvents(EventBus.java:304)
	at com.google.common.eventbus.EventBus.post(EventBus.java:275)
	at cpw.mods.fml.common.LoadController.sendEventToModContainer(LoadController.java:212)
	at cpw.mods.fml.common.LoadController.propogateStateMessage(LoadController.java:190)
	at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method)
	at sun.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:62)
	at sun.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43)
	at java.lang.reflect.Method.invoke(Method.java:497)
	at com.google.common.eventbus.EventSubscriber.handleEvent(EventSubscriber.java:74)
	at com.google.common.eventbus.SynchronizedEventSubscriber.handleEvent(SynchronizedEventSubscriber.java:47)
	at com.google.common.eventbus.EventBus.dispatch(EventBus.java:322)
	at com.google.common.eventbus.EventBus.dispatchQueuedEvents(EventBus.java:304)
	at com.google.common.eventbus.EventBus.post(EventBus.java:275)
	at cpw.mods.fml.common.LoadController.distributeStateMessage(LoadController.java:119)
	at cpw.mods.fml.common.Loader.loadMods(Loader.java:513)
	... 10 more
Caused by: java.lang.ClassNotFoundException: codechicken.multipart.BlockMultipart
	at net.minecraft.launchwrapper.LaunchClassLoader.findClass(LaunchClassLoader.java:191)
	at java.lang.ClassLoader.loadClass(ClassLoader.java:424)
	at java.lang.ClassLoader.loadClass(ClassLoader.java:357)
	... 35 more
Caused by: java.lang.NullPointerException
	at net.minecraft.launchwrapper.LaunchClassLoader.findClass(LaunchClassLoader.java:182)
	... 37 more


A detailed walkthrough of the error, its code path and all known details is as follows:
---------------------------------------------------------------------------------------

-- System Details --
Details:
	Minecraft Version: 1.7.10
	Operating System: Windows 10 (amd64) version 10.0
	Java Version: 1.8.0_51, Oracle Corporation
	Java VM Version: Java HotSpot(TM) 64-Bit Server VM (mixed mode), Oracle Corporation
	Memory: 611248984 bytes (582 MB) / 872415232 bytes (832 MB) up to 2147483648 bytes (2048 MB)
	JVM Flags: 8 total; -XX:HeapDumpPath=MojangTricksIntelDriversForPerformance_javaw.exe_minecraft.exe.heapdump -Xmx2G -XX:+UnlockExperimentalVMOptions -XX:+UseG1GC -XX:G1NewSizePercent=20 -XX:G1ReservePercent=20 -XX:MaxGCPauseMillis=50 -XX:G1HeapRegionSize=32M
	AABB Pool Size: 0 (0 bytes; 0 MB) allocated, 0 (0 bytes; 0 MB) used
	IntCache: cache: 0, tcache: 0, allocated: 0, tallocated: 0
	FML: MCP v9.05 FML v7.10.99.99 Minecraft Forge 10.13.4.1558 15 mods loaded, 15 mods active
	States: 'U' = Unloaded 'L' = Loaded 'C' = Constructed 'H' = Pre-initialized 'I' = Initialized 'J' = Post-initialized 'A' = Available 'D' = Disabled 'E' = Errored
	UC	mcp{9.05} [Minecraft Coder Pack] (minecraft.jar) 
	UC	FML{7.10.99.99} [Forge Mod Loader] (forge-1.7.10-10.13.4.1558-1.7.10.jar) 
	UC	Forge{10.13.4.1558} [Minecraft Forge] (forge-1.7.10-10.13.4.1558-1.7.10.jar) 
	UC	OpenComputers|Core{1.7.4.1265} [OpenComputers (Core)] (minecraft.jar) 
	UC	mod.ymt.air.HariboteAirCraft{172v3 hiten} [HariboteAirCraft] (AirCraft-Mod-1.7.10.zip) 
	UC	hbm{1.0.27 BETA (3654)} [Hbm's Nuclear Tech] (hbm_1.0.27_X3654.jar) 
	UE	Mekanism{9.1.1} [Mekanism] (Mekanism-Mod-Core-1.7.10.jar) 
	UE	MekanismGenerators{9.1.1} [MekanismGenerators] (Mekanism-Mod-Generators-1.7.10.jar) 
	UE	MekanismTools{9.1.1} [MekanismTools] (Mekanism-Mod-Tools-1.7.10.jar) 
	UC	MCEF{0.6} [Minecraft Chromium Embedded Framework] (Minecraft-Chromium-Embedded-Framework-1.7.10.jar) 
	UC	OpenComputers{1.7.4.1265} [OpenComputers] (OpenComputers-Mod-1.7.10.jar) 
	UC	opensecurity{1.0.117} [OpenSecurity] (OpenSecurity-1.7.10-1.0-117.jar) 
	UC	parachutemod{1.7.10} [Parachute Mod] (Parachute-Mod-1.7.10.jar) 
	UC	PneumaticCraft{1.12.7-152} [PneumaticCraft] (PneumaticCraft-1.7.10-1.12.7-152-universal.jar) 
	UC	WebDisplay{0.11} [Web Displays] (Web-Displays-Mod-1.7.10.jar) 
	GL info: ' Vendor: 'ATI Technologies Inc.' Version: '4.6.14760 Compatibility Profile Context 21.2.3 27.20.14535.3005' Renderer: 'AMD Radeon R9 200 / HD 7900 Series'
