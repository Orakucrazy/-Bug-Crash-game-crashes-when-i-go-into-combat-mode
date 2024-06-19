# -Bug-Crash-game-crashes-when-i-go-into-combat-mode
I was trying to make a minecraft modpack for just me and my friends and wanted to add epic fight but everytime i tested it I would crash and then I tried with another modpack that only has epic fight mods and its add-ons and it worked perfectly and just can't understand why i keep crashing when i try in the other modpack. 
---- Minecraft Crash Report ----
// Why did you do that?

Time: 2024-06-19 11:06:01
Description: Unexpected error

java.lang.ArrayIndexOutOfBoundsException: Index 12 out of bounds for length 12
	at yesman.epicfight.world.capabilities.entitypatch.player.PlayerPatch.getSkill(PlayerPatch.java:221) ~[EpicFight-20.7.4.jar%23538!/:20.7.4] {re:mixin,re:classloading,pl:mixin:A}
	at yesman.epicfight.client.gui.BattleModeGui.renderGui(BattleModeGui.java:136) ~[EpicFight-20.7.4.jar%23538!/:20.7.4] {re:classloading,pl:runtimedistcleaner:A}
	at yesman.epicfight.client.events.engine.RenderEngine$Events.renderGui(RenderEngine.java:574) ~[EpicFight-20.7.4.jar%23538!/:20.7.4] {re:mixin,re:classloading,pl:mixin:A}
	at yesman.epicfight.client.events.engine.__Events_renderGui_Pre.invoke(.dynamic) ~[EpicFight-20.7.4.jar%23538!/:20.7.4] {re:classloading,pl:eventbus:B}
	at net.minecraftforge.eventbus.ASMEventHandler.invoke(ASMEventHandler.java:73) ~[eventbus-6.0.5.jar%2387!/:?] {}
	at net.minecraftforge.eventbus.EventBus.post(EventBus.java:315) ~[eventbus-6.0.5.jar%2387!/:?] {}
	at net.minecraftforge.eventbus.EventBus.post(EventBus.java:296) ~[eventbus-6.0.5.jar%2387!/:?] {}
	at net.minecraftforge.client.gui.overlay.ForgeGui.m_280421_(ForgeGui.java:112) ~[forge-1.20.1-47.3.0-universal.jar%23711!/:?] {re:classloading,re:mixin}
	at net.minecraft.client.renderer.GameRenderer.m_109093_(GameRenderer.java:945) ~[client-1.20.1-20230612.114412-srg.jar%23706!/:?] {re:mixin,pl:accesstransformer:B,pl:runtimedistcleaner:A,re:classloading,pl:accesstransformer:B,pl:mixin:APP:moonlight-common.mixins.json:GameRendererMixin,pl:mixin:APP:pehkui.mixins.json:reach.client.compat1202minus.GameRendererMixin,pl:mixin:APP:supplementaries-common.mixins.json:GameRendererMixin,pl:mixin:APP:loot_journal.mixins.json:GameRendererMixin,pl:mixin:APP:pehkui.mixins.json:client.compat1193plus.GameRendererMixin,pl:mixin:APP:pehkui.mixins.json:client.compat1204minus.compat1193plus.GameRendererMixin,pl:mixin:APP:mixins.cofhcore.json:GameRendererMixin,pl:mixin:APP:zeta_forge.mixins.json:client.GameRenderMixin,pl:mixin:APP:ad_astra-common.mixins.json:client.GameRendererMixin,pl:mixin:APP:ars_nouveau.mixins.json:GameRendererMixin,pl:mixin:APP:railways-common.mixins.json:client.MixinGameRenderer,pl:mixin:APP:railways-common.mixins.json:conductor_possession.MixinGameRenderer,pl:mixin:APP:witherstormmod.mixins.json:IMixinGameRenderer,pl:mixin:APP:witherstormmod.mixins.json:MixinGameRenderer,pl:mixin:APP:brewery-common.mixins.json:GameRendererMixin,pl:mixin:APP:mixins.artifacts.common.json:item.wearable.nightvisiongoggles.client.GameRendererMixin,pl:mixin:APP:crackerslib.mixins.json:MixinGameRendererAccessor,pl:mixin:APP:create.mixins.json:accessor.GameRendererAccessor,pl:mixin:APP:create.mixins.json:client.GameRendererMixin,pl:mixin:APP:securitycraft.mixins.json:camera.GameRendererMixin,pl:mixin:A,pl:runtimedistcleaner:A}
	at net.minecraft.client.Minecraft.m_91383_(Minecraft.java:1146) ~[client-1.20.1-20230612.114412-srg.jar%23706!/:?] {re:mixin,pl:accesstransformer:B,pl:runtimedistcleaner:A,re:classloading,pl:accesstransformer:B,pl:mixin:APP:neat.mixins.json:MinecraftMixin,pl:mixin:APP:modernfix-common.mixins.json:bugfix.concurrency.MinecraftMixin,pl:mixin:APP:modernfix-common.mixins.json:bugfix.world_leaks.MinecraftMixin,pl:mixin:APP:modernfix-common.mixins.json:perf.dedicated_reload_executor.MinecraftMixin,pl:mixin:APP:modernfix-common.mixins.json:perf.blast_search_trees.MinecraftMixin,pl:mixin:APP:modernfix-common.mixins.json:feature.measure_time.MinecraftMixin,pl:mixin:APP:modernfix-forge.mixins.json:feature.measure_time.MinecraftMixin_Forge,pl:mixin:APP:balm.mixins.json:MinecraftMixin,pl:mixin:APP:immersive_armors.mixins.json:MixinMinecraftClient,pl:mixin:APP:mixins.codechickenlib.json:MinecraftMixin,pl:mixin:APP:flywheel.mixins.json:PausedPartialTickAccessor,pl:mixin:APP:ars_nouveau.mixins.json:light.ClientMixin,pl:mixin:APP:bookshelf.common.mixins.json:accessors.client.AccessorMinecraft,pl:mixin:APP:railways-common.mixins.json:conductor_possession.MixinMinecraft,pl:mixin:APP:carryon.mixins.json:MinecraftMixin,pl:mixin:APP:betterthirdperson.mixins.json:MinecraftMixin,pl:mixin:APP:witherstormmod.mixins.json:MixinMinecraft,pl:mixin:APP:architectury.mixins.json:MixinMinecraft,pl:mixin:APP:brewery-common.mixins.json:rope.PickMixin,pl:mixin:APP:azurelib.forge.mixins.json:MinecraftMixin,pl:mixin:APP:moonlight-common.mixins.json:MinecraftMixin,pl:mixin:APP:iceberg.mixins.json:MinecraftMixin,pl:mixin:APP:mixins.irons_spellbooks.json:MinecraftMixin,pl:mixin:APP:create.mixins.json:client.WindowResizeMixin,pl:mixin:APP:securitycraft.mixins.json:camera.MinecraftMixin,pl:mixin:APP:ars_nouveau.mixins.json:camera.MinecraftMixin,pl:mixin:A,pl:runtimedistcleaner:A}
	at net.minecraft.client.Minecraft.m_91374_(Minecraft.java:718) ~[client-1.20.1-20230612.114412-srg.jar%23706!/:?] {re:mixin,pl:accesstransformer:B,pl:runtimedistcleaner:A,re:classloading,pl:accesstransformer:B,pl:mixin:APP:neat.mixins.json:MinecraftMixin,pl:mixin:APP:modernfix-common.mixins.json:bugfix.concurrency.MinecraftMixin,pl:mixin:APP:modernfix-common.mixins.json:bugfix.world_leaks.MinecraftMixin,pl:mixin:APP:modernfix-common.mixins.json:perf.dedicated_reload_executor.MinecraftMixin,pl:mixin:APP:modernfix-common.mixins.json:perf.blast_search_trees.MinecraftMixin,pl:mixin:APP:modernfix-common.mixins.json:feature.measure_time.MinecraftMixin,pl:mixin:APP:modernfix-forge.mixins.json:feature.measure_time.MinecraftMixin_Forge,pl:mixin:APP:balm.mixins.json:MinecraftMixin,pl:mixin:APP:immersive_armors.mixins.json:MixinMinecraftClient,pl:mixin:APP:mixins.codechickenlib.json:MinecraftMixin,pl:mixin:APP:flywheel.mixins.json:PausedPartialTickAccessor,pl:mixin:APP:ars_nouveau.mixins.json:light.ClientMixin,pl:mixin:APP:bookshelf.common.mixins.json:accessors.client.AccessorMinecraft,pl:mixin:APP:railways-common.mixins.json:conductor_possession.MixinMinecraft,pl:mixin:APP:carryon.mixins.json:MinecraftMixin,pl:mixin:APP:betterthirdperson.mixins.json:MinecraftMixin,pl:mixin:APP:witherstormmod.mixins.json:MixinMinecraft,pl:mixin:APP:architectury.mixins.json:MixinMinecraft,pl:mixin:APP:brewery-common.mixins.json:rope.PickMixin,pl:mixin:APP:azurelib.forge.mixins.json:MinecraftMixin,pl:mixin:APP:moonlight-common.mixins.json:MinecraftMixin,pl:mixin:APP:iceberg.mixins.json:MinecraftMixin,pl:mixin:APP:mixins.irons_spellbooks.json:MinecraftMixin,pl:mixin:APP:create.mixins.json:client.WindowResizeMixin,pl:mixin:APP:securitycraft.mixins.json:camera.MinecraftMixin,pl:mixin:APP:ars_nouveau.mixins.json:camera.MinecraftMixin,pl:mixin:A,pl:runtimedistcleaner:A}
	at net.minecraft.client.main.Main.main(Main.java:218) ~[forge-47.3.0.jar:?] {re:mixin,pl:runtimedistcleaner:A,re:classloading,pl:mixin:APP:flywheel.mixins.json:ClientMainMixin,pl:mixin:A,pl:runtimedistcleaner:A}
	at jdk.internal.reflect.NativeMethodAccessorImpl.invoke0(Native Method) ~[?:?] {}
	at jdk.internal.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:77) ~[?:?] {}
	at jdk.internal.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43) ~[?:?] {}
	at java.lang.reflect.Method.invoke(Method.java:568) ~[?:?] {re:mixin}
	at net.minecraftforge.fml.loading.targets.CommonLaunchHandler.runTarget(CommonLaunchHandler.java:111) ~[fmlloader-1.20.1-47.3.0.jar:?] {}
	at net.minecraftforge.fml.loading.targets.CommonLaunchHandler.clientService(CommonLaunchHandler.java:99) ~[fmlloader-1.20.1-47.3.0.jar:?] {}
	at net.minecraftforge.fml.loading.targets.CommonClientLaunchHandler.lambda$makeService$0(CommonClientLaunchHandler.java:25) ~[fmlloader-1.20.1-47.3.0.jar:?] {}
	at cpw.mods.modlauncher.LaunchServiceHandlerDecorator.launch(LaunchServiceHandlerDecorator.java:30) ~[modlauncher-10.0.9.jar:?] {}
	at cpw.mods.modlauncher.LaunchServiceHandler.launch(LaunchServiceHandler.java:53) ~[modlauncher-10.0.9.jar:?] {}
	at cpw.mods.modlauncher.LaunchServiceHandler.launch(LaunchServiceHandler.java:71) ~[modlauncher-10.0.9.jar:?] {}
	at cpw.mods.modlauncher.Launcher.run(Launcher.java:108) ~[modlauncher-10.0.9.jar:?] {}
	at cpw.mods.modlauncher.Launcher.main(Launcher.java:78) ~[modlauncher-10.0.9.jar:?] {}
	at cpw.mods.modlauncher.BootstrapLaunchConsumer.accept(BootstrapLaunchConsumer.java:26) ~[modlauncher-10.0.9.jar:?] {}
	at cpw.mods.modlauncher.BootstrapLaunchConsumer.accept(BootstrapLaunchConsumer.java:23) ~[modlauncher-10.0.9.jar:?] {}
	at cpw.mods.bootstraplauncher.BootstrapLauncher.main(BootstrapLauncher.java:141) ~[bootstraplauncher-1.1.2.jar:?] {}


A detailed walkthrough of the error, its code path and all known details is as follows:
---------------------------------------------------------------------------------------

-- Head --
Thread: Render thread
Suspected Mod: 
	Epic Fight (epicfight), Version: 20.7.4
		at TRANSFORMER/epicfight@20.7.4/yesman.epicfight.world.capabilities.entitypatch.player.PlayerPatch.getSkill(PlayerPatch.java:221)
Stacktrace:
	at yesman.epicfight.world.capabilities.entitypatch.player.PlayerPatch.getSkill(PlayerPatch.java:221) ~[EpicFight-20.7.4.jar%23538!/:20.7.4] {re:mixin,re:classloading,pl:mixin:A}
	at yesman.epicfight.client.gui.BattleModeGui.renderGui(BattleModeGui.java:136) ~[EpicFight-20.7.4.jar%23538!/:20.7.4] {re:classloading,pl:runtimedistcleaner:A}
	at yesman.epicfight.client.events.engine.RenderEngine$Events.renderGui(RenderEngine.java:574) ~[EpicFight-20.7.4.jar%23538!/:20.7.4] {re:mixin,re:classloading,pl:mixin:A}
	at yesman.epicfight.client.events.engine.__Events_renderGui_Pre.invoke(.dynamic) ~[EpicFight-20.7.4.jar%23538!/:20.7.4] {re:classloading,pl:eventbus:B}
	at net.minecraftforge.eventbus.ASMEventHandler.invoke(ASMEventHandler.java:73) ~[eventbus-6.0.5.jar%2387!/:?] {}
	at net.minecraftforge.eventbus.EventBus.post(EventBus.java:315) ~[eventbus-6.0.5.jar%2387!/:?] {}
	at net.minecraftforge.eventbus.EventBus.post(EventBus.java:296) ~[eventbus-6.0.5.jar%2387!/:?] {}
	at net.minecraftforge.client.gui.overlay.ForgeGui.m_280421_(ForgeGui.java:112) ~[forge-1.20.1-47.3.0-universal.jar%23711!/:?] {re:classloading,re:mixin}
-- Affected level --
Details:
	All players: 1 total; [LocalPlayer['Orakucrazy'/394, l='ClientLevel', x=-154.76, y=72.00, z=-59.69]]
	Chunk stats: 961, 505
	Level dimension: minecraft:overworld
	Level spawn location: World: (-160,79,-64), Section: (at 0,15,0 in -10,4,-4; chunk contains blocks -160,-64,-64 to -145,319,-49), Region: (-1,-1; contains chunks -32,-32 to -1,-1, blocks -512,-64,-512 to -1,319,-1)
	Level time: 418 game time, 418 day time
	Server brand: forge
	Server type: Integrated singleplayer server
Stacktrace:
	at net.minecraft.client.multiplayer.ClientLevel.m_6026_(ClientLevel.java:455) ~[client-1.20.1-20230612.114412-srg.jar%23706!/:?] {re:mixin,pl:accesstransformer:B,pl:runtimedistcleaner:A,re:classloading,pl:accesstransformer:B,pl:mixin:APP:supplementaries-common.mixins.json:ClientLevelMixin,pl:mixin:APP:pehkui.mixins.json:client.ClientWorldMixin,pl:mixin:APP:flywheel.mixins.json:ClientLevelMixin,pl:mixin:APP:citadel.mixins.json:client.ClientLevelMixin,pl:mixin:APP:witherstormmod.mixins.json:MixinClientLevel,pl:mixin:APP:architectury.mixins.json:MixinClientLevel,pl:mixin:A,pl:runtimedistcleaner:A}
	at net.minecraft.client.Minecraft.m_91354_(Minecraft.java:2319) ~[client-1.20.1-20230612.114412-srg.jar%23706!/:?] {re:mixin,pl:accesstransformer:B,pl:runtimedistcleaner:A,re:classloading,pl:accesstransformer:B,pl:mixin:APP:neat.mixins.json:MinecraftMixin,pl:mixin:APP:modernfix-common.mixins.json:bugfix.concurrency.MinecraftMixin,pl:mixin:APP:modernfix-common.mixins.json:bugfix.world_leaks.MinecraftMixin,pl:mixin:APP:modernfix-common.mixins.json:perf.dedicated_reload_executor.MinecraftMixin,pl:mixin:APP:modernfix-common.mixins.json:perf.blast_search_trees.MinecraftMixin,pl:mixin:APP:modernfix-common.mixins.json:feature.measure_time.MinecraftMixin,pl:mixin:APP:modernfix-forge.mixins.json:feature.measure_time.MinecraftMixin_Forge,pl:mixin:APP:balm.mixins.json:MinecraftMixin,pl:mixin:APP:immersive_armors.mixins.json:MixinMinecraftClient,pl:mixin:APP:mixins.codechickenlib.json:MinecraftMixin,pl:mixin:APP:flywheel.mixins.json:PausedPartialTickAccessor,pl:mixin:APP:ars_nouveau.mixins.json:light.ClientMixin,pl:mixin:APP:bookshelf.common.mixins.json:accessors.client.AccessorMinecraft,pl:mixin:APP:railways-common.mixins.json:conductor_possession.MixinMinecraft,pl:mixin:APP:carryon.mixins.json:MinecraftMixin,pl:mixin:APP:betterthirdperson.mixins.json:MinecraftMixin,pl:mixin:APP:witherstormmod.mixins.json:MixinMinecraft,pl:mixin:APP:architectury.mixins.json:MixinMinecraft,pl:mixin:APP:brewery-common.mixins.json:rope.PickMixin,pl:mixin:APP:azurelib.forge.mixins.json:MinecraftMixin,pl:mixin:APP:moonlight-common.mixins.json:MinecraftMixin,pl:mixin:APP:iceberg.mixins.json:MinecraftMixin,pl:mixin:APP:mixins.irons_spellbooks.json:MinecraftMixin,pl:mixin:APP:create.mixins.json:client.WindowResizeMixin,pl:mixin:APP:securitycraft.mixins.json:camera.MinecraftMixin,pl:mixin:APP:ars_nouveau.mixins.json:camera.MinecraftMixin,pl:mixin:A,pl:runtimedistcleaner:A}
	at net.minecraft.client.Minecraft.m_91374_(Minecraft.java:740) ~[client-1.20.1-20230612.114412-srg.jar%23706!/:?] {re:mixin,pl:accesstransformer:B,pl:runtimedistcleaner:A,re:classloading,pl:accesstransformer:B,pl:mixin:APP:neat.mixins.json:MinecraftMixin,pl:mixin:APP:modernfix-common.mixins.json:bugfix.concurrency.MinecraftMixin,pl:mixin:APP:modernfix-common.mixins.json:bugfix.world_leaks.MinecraftMixin,pl:mixin:APP:modernfix-common.mixins.json:perf.dedicated_reload_executor.MinecraftMixin,pl:mixin:APP:modernfix-common.mixins.json:perf.blast_search_trees.MinecraftMixin,pl:mixin:APP:modernfix-common.mixins.json:feature.measure_time.MinecraftMixin,pl:mixin:APP:modernfix-forge.mixins.json:feature.measure_time.MinecraftMixin_Forge,pl:mixin:APP:balm.mixins.json:MinecraftMixin,pl:mixin:APP:immersive_armors.mixins.json:MixinMinecraftClient,pl:mixin:APP:mixins.codechickenlib.json:MinecraftMixin,pl:mixin:APP:flywheel.mixins.json:PausedPartialTickAccessor,pl:mixin:APP:ars_nouveau.mixins.json:light.ClientMixin,pl:mixin:APP:bookshelf.common.mixins.json:accessors.client.AccessorMinecraft,pl:mixin:APP:railways-common.mixins.json:conductor_possession.MixinMinecraft,pl:mixin:APP:carryon.mixins.json:MinecraftMixin,pl:mixin:APP:betterthirdperson.mixins.json:MinecraftMixin,pl:mixin:APP:witherstormmod.mixins.json:MixinMinecraft,pl:mixin:APP:architectury.mixins.json:MixinMinecraft,pl:mixin:APP:brewery-common.mixins.json:rope.PickMixin,pl:mixin:APP:azurelib.forge.mixins.json:MinecraftMixin,pl:mixin:APP:moonlight-common.mixins.json:MinecraftMixin,pl:mixin:APP:iceberg.mixins.json:MinecraftMixin,pl:mixin:APP:mixins.irons_spellbooks.json:MinecraftMixin,pl:mixin:APP:create.mixins.json:client.WindowResizeMixin,pl:mixin:APP:securitycraft.mixins.json:camera.MinecraftMixin,pl:mixin:APP:ars_nouveau.mixins.json:camera.MinecraftMixin,pl:mixin:A,pl:runtimedistcleaner:A}
	at net.minecraft.client.main.Main.main(Main.java:218) ~[forge-47.3.0.jar:?] {re:mixin,pl:runtimedistcleaner:A,re:classloading,pl:mixin:APP:flywheel.mixins.json:ClientMainMixin,pl:mixin:A,pl:runtimedistcleaner:A}
	at jdk.internal.reflect.NativeMethodAccessorImpl.invoke0(Native Method) ~[?:?] {}
	at jdk.internal.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:77) ~[?:?] {}
	at jdk.internal.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43) ~[?:?] {}
	at java.lang.reflect.Method.invoke(Method.java:568) ~[?:?] {re:mixin}
	at net.minecraftforge.fml.loading.targets.CommonLaunchHandler.runTarget(CommonLaunchHandler.java:111) ~[fmlloader-1.20.1-47.3.0.jar:?] {}
	at net.minecraftforge.fml.loading.targets.CommonLaunchHandler.clientService(CommonLaunchHandler.java:99) ~[fmlloader-1.20.1-47.3.0.jar:?] {}
	at net.minecraftforge.fml.loading.targets.CommonClientLaunchHandler.lambda$makeService$0(CommonClientLaunchHandler.java:25) ~[fmlloader-1.20.1-47.3.0.jar:?] {}
	at cpw.mods.modlauncher.LaunchServiceHandlerDecorator.launch(LaunchServiceHandlerDecorator.java:30) ~[modlauncher-10.0.9.jar:?] {}
	at cpw.mods.modlauncher.LaunchServiceHandler.launch(LaunchServiceHandler.java:53) ~[modlauncher-10.0.9.jar:?] {}
	at cpw.mods.modlauncher.LaunchServiceHandler.launch(LaunchServiceHandler.java:71) ~[modlauncher-10.0.9.jar:?] {}
	at cpw.mods.modlauncher.Launcher.run(Launcher.java:108) ~[modlauncher-10.0.9.jar:?] {}
	at cpw.mods.modlauncher.Launcher.main(Launcher.java:78) ~[modlauncher-10.0.9.jar:?] {}
	at cpw.mods.modlauncher.BootstrapLaunchConsumer.accept(BootstrapLaunchConsumer.java:26) ~[modlauncher-10.0.9.jar:?] {}
	at cpw.mods.modlauncher.BootstrapLaunchConsumer.accept(BootstrapLaunchConsumer.java:23) ~[modlauncher-10.0.9.jar:?] {}
	at cpw.mods.bootstraplauncher.BootstrapLauncher.main(BootstrapLauncher.java:141) ~[bootstraplauncher-1.1.2.jar:?] {}


-- Last reload --
Details:
	Reload number: 1
	Reload reason: initial
	Finished: Yes
	Packs: vanilla, mod_resources, Moonlight Mods Dynamic Assets, black_icons, builtin/builtin_resource_packs/legacy_dead_king_resource_pack, create:legacy_copper, file/EclecticTrove-1.20.1-1.3.0.zip, file/Iron's_3D_Spell_book_v2.0.zip, file/Pretty_Pipez_1_20.zip, file/Trinkets_OffhandFix_1.2+1.20.1.zip, file/[1.19-1.20] Yuushya Release 0.18.2.zip, file/[1.4.1] Enhanced Boss Bars.zip, file/sebas_aquamirae_1.20.zip, file/sebas_born_in_chaos_1.3.zip, file/sebas_cataclysm_1.3.zip, file/waystones_1.20.zip, supplementaries:darker_ropes, file/Yuushya Foliage Addon 1.3.zip, file/EFMxIronsV2.0.zip, file/SkyVillages-WaystonesCompat-1.20.1-1.0.3-fabric.zip, file/guard_epic_rewritten_1.0 fix fix.zip, file/Dark Souls Armory Hotfix.zip

-- System Details --
Details:
	Minecraft Version: 1.20.1
	Minecraft Version ID: 1.20.1
	Operating System: Windows 11 (amd64) version 10.0
	Java Version: 17.0.8, Microsoft
	Java VM Version: OpenJDK 64-Bit Server VM (mixed mode), Microsoft
	Memory: 2722041208 bytes (2595 MiB) / 11324620800 bytes (10800 MiB) up to 15904800768 bytes (15168 MiB)
	CPUs: 12
	Processor Vendor: AuthenticAMD
	Processor Name: AMD Ryzen 5 5600X 6-Core Processor             
	Identifier: AuthenticAMD Family 25 Model 33 Stepping 0
	Microarchitecture: Zen 3
	Frequency (GHz): 3.70
	Number of physical packages: 1
	Number of physical CPUs: 6
	Number of logical CPUs: 12
	Graphics card #0 name: NVIDIA GeForce RTX 3060 Ti
	Graphics card #0 vendor: NVIDIA (0x10de)
	Graphics card #0 VRAM (MB): 4095.00
	Graphics card #0 deviceId: 0x2489
	Graphics card #0 versionInfo: DriverVersion=32.0.15.5599
	Memory slot #0 capacity (MB): 8192.00
	Memory slot #0 clockSpeed (GHz): 2.67
	Memory slot #0 type: DDR4
	Memory slot #1 capacity (MB): 8192.00
	Memory slot #1 clockSpeed (GHz): 2.67
	Memory slot #1 type: DDR4
	Virtual memory max (MB): 40986.15
	Virtual memory used (MB): 35762.64
	Swap memory total (MB): 24676.91
	Swap memory used (MB): 4208.64
	JVM Flags: 4 total; -XX:HeapDumpPath=MojangTricksIntelDriversForPerformance_javaw.exe_minecraft.exe.heapdump -Xss1M -Xmx15168m -Xms256m
	Launched Version: forge-47.3.0
	Backend library: LWJGL version 3.3.1 build 7
	Backend API: NVIDIA GeForce RTX 3060 Ti/PCIe/SSE2 GL version 4.6.0 NVIDIA 555.99, NVIDIA Corporation
	Window size: 2560x1351
	GL Caps: Using framebuffer using OpenGL 3.2
	GL debug messages: 
	Using VBOs: Yes
	Is Modded: Definitely; Client brand changed to 'forge'; Server brand changed to 'forge'
	Type: Integrated Server (map_client.txt)
	Graphics mode: fancy
	Resource Packs: vanilla, mod_resources, Moonlight Mods Dynamic Assets, black_icons, builtin/builtin_resource_packs/legacy_dead_king_resource_pack, create:legacy_copper, file/EclecticTrove-1.20.1-1.3.0.zip, file/Iron's_3D_Spell_book_v2.0.zip, file/Pretty_Pipez_1_20.zip, file/Trinkets_OffhandFix_1.2+1.20.1.zip, file/[1.19-1.20] Yuushya Release 0.18.2.zip, file/[1.4.1] Enhanced Boss Bars.zip, file/sebas_aquamirae_1.20.zip, file/sebas_born_in_chaos_1.3.zip, file/sebas_cataclysm_1.3.zip, file/waystones_1.20.zip, supplementaries:darker_ropes, file/Yuushya Foliage Addon 1.3.zip (incompatible), file/EFMxIronsV2.0.zip (incompatible), file/SkyVillages-WaystonesCompat-1.20.1-1.0.3-fabric.zip (incompatible), file/guard_epic_rewritten_1.0 fix fix.zip (incompatible), file/Dark Souls Armory Hotfix.zip
	Current Language: en_us
	CPU: 12x AMD Ryzen 5 5600X 6-Core Processor 
	Server Running: true
	Player Count: 1 / 8; [ServerPlayer['Orakucrazy'/394, l='ServerLevel[New World]', x=-154.76, y=72.00, z=-59.69]]
	Data Packs: vanilla, mod:ftbessentials (incompatible), mod:supermartijn642configlib (incompatible), mod:createdeco (incompatible), mod:playeranimator (incompatible), mod:botarium (incompatible), mod:mcwwindows, mod:stalwart_dungeons, mod:neat, mod:forgeendertech, mod:modernfix (incompatible), mod:yungsapi, mod:powah (incompatible), mod:cabletiers, mod:lootbeams (incompatible), mod:guardvillagers (incompatible), mod:chancecubes, mod:apotheosis (incompatible), mod:ec_apotheosis_plugin (incompatible), mod:create_new_age, mod:balm, mod:immersive_armors (incompatible), mod:jeresources, mod:chat_heads (incompatible), mod:betterfortresses, mod:cloth_config (incompatible), mod:shetiphiancore, mod:supplementaries, mod:structure_gel, mod:lmft (incompatible), mod:corpse, mod:advancementplaques (incompatible), mod:handcrafted (incompatible), mod:repurposed_structures, mod:apothic_amendments__enchanting, mod:loot_journal, mod:explorify (incompatible), mod:ironfurnaces, mod:mcwtrpdoors, mod:apotheosis_ascended, mod:supermartijn642corelib, mod:yungsbridges, mod:resourcefulconfig (incompatible), mod:curios (incompatible), mod:advancednetherite, mod:searchables (incompatible), mod:advgenerators, mod:attributeslib (incompatible), mod:epic_stats_mod_remastered, mod:bettervillage, mod:extrastorage, mod:mcwroofs, mod:indestructible, mod:cfm, mod:apothiccurios (incompatible), mod:flib, mod:betterendisland, mod:l2library (incompatible), mod:toms_storage (incompatible), mod:codechickenlib (incompatible), mod:cataclysm_ut, mod:arsmagicalegacy, mod:apothic_sups_enchanting, mod:sliceanddice (incompatible), mod:mcwlights, mod:betterjungletemples, mod:elytraslot (incompatible), mod:mowziesmobs, mod:doubledoors, mod:harvestwithease, mod:jei, mod:visualworkbench, mod:pehkui (incompatible), mod:libraryferret, mod:goblintraders (incompatible), mod:epicsamurai (incompatible), mod:mekanism, mod:caelus (incompatible), mod:bdlib, mod:epicfight (incompatible), mod:refm, mod:wom (incompatible), mod:integrated_api, mod:naturescompass, mod:epherolib (incompatible), mod:neruina (incompatible), mod:fusion, mod:epictweaks (incompatible), mod:extradisks, mod:edivadlib, mod:puzzlesaccessapi, mod:forge, mod:ironchest, mod:dungeons_arise, mod:zerocore (incompatible), mod:cofh_core, mod:thermal, mod:thermal_integration, mod:thermal_innovation, mod:thermal_foundation, mod:thermal_locomotion, mod:thermal_dynamics, mod:smoothchunk (incompatible), mod:voicechat (incompatible), mod:adlods, mod:spectrelib (incompatible), mod:domum_ornamentum, mod:kotlinforforge (incompatible), mod:pipez, mod:notenoughanimations, mod:flywheel, mod:createoreexcavation (incompatible), mod:soulslikeuniverse, mod:itemcollectors (incompatible), mod:croptopia (incompatible), mod:thermal_cultivation, mod:polymorph (incompatible), mod:justenoughprofessions, mod:securitycraft, mod:zeta (incompatible), mod:structurize, mod:oceansdelight (incompatible), mod:appleskin (incompatible), mod:moremobvariants, mod:lootr, mod:connectedglass, mod:puzzleslib, mod:aquaculture, mod:efm_compat, mod:cosmeticarmorreworked, mod:chunksending (incompatible), mod:aquamirae (incompatible), mod:cristellib (incompatible), mod:ad_astra (incompatible), mod:rsrequestify (incompatible), mod:weaponmaster_ydm (incompatible), mod:effs, mod:skyvillages (incompatible), mod:kuma_api (incompatible), mod:betterwitchhuts, mod:geckolib, mod:ars_nouveau (incompatible), mod:ec_ars_plugin (incompatible), mod:shifu_epic_fight_skill_recipe, mod:knightsnmages, mod:illagerinvasion, mod:betteroceanmonuments, mod:connectivity (incompatible), mod:sophisticatedcore (incompatible), mod:gpumemleakfix (incompatible), mod:insanelib, mod:cookingforblockheads, mod:controlling (incompatible), mod:prism (incompatible), mod:placebo (incompatible), mod:citadel (incompatible), mod:alexsmobs (incompatible), mod:iceandfire, mod:mixinextras (incompatible), mod:ec_es_plugin (incompatible), mod:expanded_combat (incompatible), mod:ec_ef_plugin (incompatible), mod:bookshelf, mod:sophisticatedbackpacks (incompatible), mod:create_dragon_lib (incompatible), mod:relics, mod:waddles, mod:takesapillage (incompatible), mod:progressivebosses, mod:mcwdoors, mod:bygonenether (incompatible), mod:railways, mod:mekanismgenerators, mod:carryon (incompatible), mod:shieldexp (incompatible), mod:dummmmmmy (incompatible), mod:twilightforest, mod:rsinfinitybooster (incompatible), mod:refinedstorage, mod:farmersdelight, mod:ends_delight, mod:endersdelight, mod:endrem (incompatible), mod:mcwfences, mod:born_in_chaos_v1, mod:lionfishapi (incompatible), mod:dungeons_enhanced, mod:cataclysm (incompatible), mod:patchouli (incompatible), mod:ars_additions (incompatible), mod:blockui, mod:multipiston, mod:collective, mod:cerbons_api, mod:villagertools (incompatible), mod:thermal_expansion, mod:betterthirdperson, mod:witherstormmod, mod:ftbultimine (incompatible), mod:betterstrongholds, mod:resourcefullib (incompatible), mod:mekanismtools, mod:twilightdelight (incompatible), mod:spartanweaponry, mod:architectury (incompatible), mod:doapi (incompatible), mod:ftblibrary (incompatible), mod:ftbteams (incompatible), mod:brewery (incompatible), mod:yuushya, mod:cupboard (incompatible), mod:bigreactors (incompatible), mod:framework, mod:smallships (incompatible), mod:t_and_t (incompatible), mod:cucumber, mod:amendments (incompatible), mod:ars_extended_glyphs (incompatible), mod:sophisticatedstorage (incompatible), mod:octolib, mod:conjurer_illager (incompatible), mod:obscure_api (incompatible), mod:create, mod:delightful (incompatible), mod:create_central_kitchen (incompatible), mod:ars_creo (incompatible), mod:waystones, mod:structory, mod:mcwpaintings, mod:comforts (incompatible), mod:artifacts, mod:crackerslib (incompatible), mod:decorative_blocks, mod:magistuarmory (incompatible), mod:magistuarmoryaddon (incompatible), mod:dungeoncrawl, mod:mcjtylib, mod:rftoolsbase, mod:rftoolspower, mod:betterdeserttemples, mod:explorerscompass, mod:mahoutsukai, mod:bosses_of_mass_destruction, mod:azurelib, mod:enderstorage (incompatible), mod:watut, mod:ftbchunks (incompatible), mod:brandonscore (incompatible), mod:draconicevolution, mod:friendsandfoes (incompatible), mod:mysticalagriculture, mod:mysticalagradditions, mod:ars_trinkets (incompatible), mod:moonlight (incompatible), mod:titanium (incompatible), mod:mysterious_mountain_lib (incompatible), mod:corn_delight (incompatible), mod:mixinsquared (incompatible), mod:jade (incompatible), mod:forbidden_arcanus (incompatible), mod:nethersdelight, mod:easy_villagers, mod:iceberg (incompatible), mod:legendarytooltips (incompatible), mod:brutalbosses (incompatible), mod:create_sa, mod:storagedrawers (incompatible), mod:fluxnetworks (incompatible), mod:ars_elemental (incompatible), mod:irons_spellbooks, mod:additional_attributes (incompatible), mod:betterchunkloading (incompatible), mod:coroutil (incompatible), mod:epic_fight_battle_styles (incompatible), mod:alexsdelight, mod:ferritecore (incompatible), mod:solcarrot (incompatible), mod:functionalstorage, mod:charmofundying (incompatible), mod:refinedstorageaddons, mod:refinedpolymorph, mod:crabbersdelight, mod:packetfixer (incompatible), mod:expandability (incompatible), mod:valhelsia_core (incompatible), mod:create_enchantment_industry (incompatible), mod:createaddition (incompatible), Supplementaries Generated Pack, T&T Waystone Patch Pack (incompatible), create_central_kitchen:corn_delight (incompatible), create_central_kitchen:ends_delight (incompatible), create_central_kitchen:farmersdelight (incompatible)
	Enabled Feature Flags: minecraft:vanilla
	World Generation: Experimental
	ModLauncher: 10.0.9+10.0.9+main.dcd20f30
	ModLauncher launch target: forgeclient
	ModLauncher naming: srg
	ModLauncher services: 
		mixin-0.8.5.jar mixin PLUGINSERVICE 
		eventbus-6.0.5.jar eventbus PLUGINSERVICE 
		fmlloader-1.20.1-47.3.0.jar slf4jfixer PLUGINSERVICE 
		fmlloader-1.20.1-47.3.0.jar object_holder_definalize PLUGINSERVICE 
		fmlloader-1.20.1-47.3.0.jar runtime_enum_extender PLUGINSERVICE 
		fmlloader-1.20.1-47.3.0.jar capability_token_subclass PLUGINSERVICE 
		accesstransformers-8.0.4.jar accesstransformer PLUGINSERVICE 
		fmlloader-1.20.1-47.3.0.jar runtimedistcleaner PLUGINSERVICE 
		modlauncher-10.0.9.jar mixin TRANSFORMATIONSERVICE 
		modlauncher-10.0.9.jar fml TRANSFORMATIONSERVICE 
	FML Language Providers: 
		minecraft@1.0
		kotlinforforge@4.11.0
		javafml@null
		lowcodefml@null
		kotori_scala@3.3.1-build-0
	Mod List: 
		ftb-essentials-forge-2001.2.2.jar                 |FTB Essentials                |ftbessentials                 |2001.2.2            |DONE      |Manifest: NOSIGNATURE
		supermartijn642configlib-1.1.8-forge-mc1.20.jar   |SuperMartijn642's Config Libra|supermartijn642configlib      |1.1.8               |DONE      |Manifest: NOSIGNATURE
		createdeco-2.0.2-1.20.1-forge.jar                 |Create Deco                   |createdeco                    |2.0.2-1.20.1-forge  |DONE      |Manifest: NOSIGNATURE
		player-animation-lib-forge-1.0.2-rc1+1.20.jar     |Player Animator               |playeranimator                |1.0.2-rc1+1.20      |DONE      |Manifest: NOSIGNATURE
		botarium-forge-1.20.1-2.3.3.jar                   |Botarium                      |botarium                      |2.3.3               |DONE      |Manifest: NOSIGNATURE
		mcw-windows-2.2.1-mc1.20.1forge.jar               |Macaw's Windows               |mcwwindows                    |2.2.1               |DONE      |Manifest: NOSIGNATURE
		stalwart-dungeons-1.20.1-1.2.8.jar                |Stalwart Dungeons             |stalwart_dungeons             |1.2.8               |DONE      |Manifest: NOSIGNATURE
		Neat-1.20-35-FORGE.jar                            |Neat                          |neat                          |1.20-35-FORGE       |DONE      |Manifest: NOSIGNATURE
		ForgeEndertech-1.20.1-11.1.4.0-build.0572.jar     |ForgeEndertech                |forgeendertech                |11.1.4.0            |DONE      |Manifest: NOSIGNATURE
		modernfix-forge-5.18.1+mc1.20.1.jar               |ModernFix                     |modernfix                     |5.18.1+mc1.20.1     |DONE      |Manifest: NOSIGNATURE
		YungsApi-1.20-Forge-4.0.5.jar                     |YUNG's API                    |yungsapi                      |1.20-Forge-4.0.5    |DONE      |Manifest: NOSIGNATURE
		Powah-5.0.5.jar                                   |Powah                         |powah                         |5.0.5               |DONE      |Manifest: NOSIGNATURE
		cabletiers-1.20.1-1.2.2.jar                       |Cable Tiers                   |cabletiers                    |1.20.1-1.2.2        |DONE      |Manifest: NOSIGNATURE
		lootbeams-1.20.1-1.2.5.jar                        |LootBeams                     |lootbeams                     |1.20.1              |DONE      |Manifest: NOSIGNATURE
		guardvillagers-1.20.1-1.6.6.jar                   |Guard Villagers               |guardvillagers                |1.20.1-1.6.6        |DONE      |Manifest: NOSIGNATURE
		ChanceCubes-1.20.1-5.0.2.489.jar                  |Chance Cubes                  |chancecubes                   |1.20.1-5.0.2.489    |DONE      |Manifest: NOSIGNATURE
		Apotheosis-1.20.1-7.3.5.jar                       |Apotheosis                    |apotheosis                    |7.3.5               |DONE      |Manifest: NOSIGNATURE
		ec_apotheosis_plugin-1.20.1-1.1.1-all.jar         |EC Compat for Apotheosis      |ec_apotheosis_plugin          |1.1.1               |DONE      |Manifest: NOSIGNATURE
		create-new-age-forge-1.20.1-1.1.2.jar             |Create: New Age               |create_new_age                |1.1.2               |DONE      |Manifest: NOSIGNATURE
		balm-forge-1.20.1-7.3.4-all.jar                   |Balm                          |balm                          |7.3.4               |DONE      |Manifest: NOSIGNATURE
		immersive_armors-1.6.1+1.20.1-forge.jar           |Immersive Armors              |immersive_armors              |1.6.1+1.20.1        |DONE      |Manifest: NOSIGNATURE
		JustEnoughResources-1.20.1-1.4.0.247.jar          |Just Enough Resources         |jeresources                   |1.4.0.247           |DONE      |Manifest: NOSIGNATURE
		chat_heads-0.12.3-forge-1.20.jar                  |Chat Heads                    |chat_heads                    |0.12.3              |DONE      |Manifest: NOSIGNATURE
		YungsBetterNetherFortresses-1.20-Forge-2.0.6.jar  |YUNG's Better Nether Fortresse|betterfortresses              |1.20-Forge-2.0.6    |DONE      |Manifest: NOSIGNATURE
		cloth-config-11.1.118-forge.jar                   |Cloth Config v10 API          |cloth_config                  |11.1.118            |DONE      |Manifest: NOSIGNATURE
		shetiphiancore-forge-1.20.1-1.3.jar               |ShetiPhian-Core               |shetiphiancore                |1.20.1-1.3          |DONE      |Manifest: NOSIGNATURE
		supplementaries-1.20-2.8.15.jar                   |Supplementaries               |supplementaries               |1.20-2.8.15         |DONE      |Manifest: NOSIGNATURE
		structure_gel-1.20.1-2.16.2.jar                   |Structure Gel API             |structure_gel                 |2.16.2              |DONE      |Manifest: NOSIGNATURE
		lmft-1.0.4+1.20.1-forge.jar                       |Load My F***ing Tags          |lmft                          |1.0.4+1.20.1        |DONE      |Manifest: NOSIGNATURE
		corpse-forge-1.20.1-1.0.12.jar                    |Corpse                        |corpse                        |1.20.1-1.0.12       |DONE      |Manifest: NOSIGNATURE
		AdvancementPlaques-1.20.1-forge-1.5.1.jar         |Advancement Plaques           |advancementplaques            |1.5.1               |DONE      |Manifest: NOSIGNATURE
		handcrafted-forge-1.20.1-3.0.6.jar                |Handcrafted                   |handcrafted                   |3.0.6               |DONE      |Manifest: NOSIGNATURE
		repurposed_structures-7.1.15+1.20.1-forge.jar     |Repurposed Structures         |repurposed_structures         |7.1.15+1.20.1-forge |DONE      |Manifest: NOSIGNATURE
		Apothic Amendments - Enchanting - 0.1.4.jar       |Apothic Amendments - Enchantin|apothic_amendments__enchanting|0.1.4               |DONE      |Manifest: NOSIGNATURE
		loot_journal-3.1.1.jar                            |Loot Journal                  |loot_journal                  |3.1.1               |DONE      |Manifest: NOSIGNATURE
		Explorify v1.5.0 f10-48.jar                       |Explorify                     |explorify                     |1.5.0               |DONE      |Manifest: NOSIGNATURE
		ironfurnaces-1.20.1-4.1.6.jar                     |Iron Furnaces                 |ironfurnaces                  |4.1.6               |DONE      |Manifest: NOSIGNATURE
		mcw-trapdoors-1.1.3-mc1.20.1forge.jar             |Macaw's Trapdoors             |mcwtrpdoors                   |1.1.3               |DONE      |Manifest: NOSIGNATURE
		Apotheosis-Ascended-1.20.1-1.2.jar                |Apotheosis Ascended           |apotheosis_ascended           |1.20-1.0            |DONE      |Manifest: NOSIGNATURE
		supermartijn642corelib-1.1.17-forge-mc1.20.1.jar  |SuperMartijn642's Core Lib    |supermartijn642corelib        |1.1.17              |DONE      |Manifest: NOSIGNATURE
		YungsBridges-1.20-Forge-4.0.3.jar                 |YUNG's Bridges                |yungsbridges                  |1.20-Forge-4.0.3    |DONE      |Manifest: NOSIGNATURE
		resourcefulconfig-forge-1.20.1-2.1.2.jar          |Resourcefulconfig             |resourcefulconfig             |2.1.2               |DONE      |Manifest: NOSIGNATURE
		curios-forge-5.9.1+1.20.1.jar                     |Curios API                    |curios                        |5.9.1+1.20.1        |DONE      |Manifest: NOSIGNATURE
		advancednetherite-forge-2.1.3-1.20.1.jar          |Advanced Netherite            |advancednetherite             |2.1.3               |DONE      |Manifest: NOSIGNATURE
		Searchables-forge-1.20.1-1.0.3.jar                |Searchables                   |searchables                   |1.0.3               |DONE      |Manifest: NOSIGNATURE
		advgenerators-1.6.0.6-mc1.20.1.jar                |Advanced Generators           |advgenerators                 |1.6.0.6             |DONE      |Manifest: NOSIGNATURE
		ApothicAttributes-1.20.1-1.3.5.jar                |Apothic Attributes            |attributeslib                 |1.3.5               |DONE      |Manifest: NOSIGNATURE
		epic_stats_mod_remastered-1.0.9f2-forge-1.20.1.jar|Epic Stats Mod Remastered     |epic_stats_mod_remastered     |1.0.9               |DONE      |Manifest: NOSIGNATURE
		bettervillage-forge-1.20.1-3.2.0.jar              |Better village                |bettervillage                 |3.1.0               |DONE      |Manifest: NOSIGNATURE
		ExtraStorage-1.20.1-4.0.7.jar                     |ExtraStorage                  |extrastorage                  |4.0.7               |DONE      |Manifest: NOSIGNATURE
		mcw-roofs-2.3.0-mc1.20.1forge.jar                 |Macaw's Roofs                 |mcwroofs                      |2.3.0               |DONE      |Manifest: NOSIGNATURE
		indestructible-20.6.7.jar                         |Indestructible                |indestructible                |20.6.7              |DONE      |Manifest: NOSIGNATURE
		cfm-forge-1.20.1-7.0.0-pre36.jar                  |MrCrayfish's Furniture Mod    |cfm                           |7.0.0-pre36         |DONE      |Manifest: 0d:78:5f:44:c0:47:0c:8c:e2:63:a3:04:43:d4:12:7d:b0:7c:35:37:dc:40:b1:c1:98:ec:51:eb:3b:3c:45:99
		ApothicCurios-1.20.1-1.0.3c.jar                   |Apothic Curios                |apothiccurios                 |1.0.3c              |DONE      |Manifest: NOSIGNATURE
		flib-1.20.1-0.0.13.jar                            |flib                          |flib                          |0.0.13              |DONE      |Manifest: 1f:47:ac:b1:61:82:96:b8:47:19:16:d2:61:81:11:60:3a:06:4b:61:31:56:7d:44:31:1e:0c:6f:22:5b:4c:ed
		YungsBetterEndIsland-1.20-Forge-2.0.6.jar         |YUNG's Better End Island      |betterendisland               |1.20-Forge-2.0.6    |DONE      |Manifest: NOSIGNATURE
		l2library-2.4.16-slim.jar                         |L2 Library                    |l2library                     |2.4.16              |DONE      |Manifest: NOSIGNATURE
		toms_storage-1.20-1.6.7.jar                       |Tom's Simple Storage Mod      |toms_storage                  |1.6.7               |DONE      |Manifest: NOSIGNATURE
		CodeChickenLib-1.20.1-4.4.0.512-universal.jar     |CodeChicken Lib               |codechickenlib                |4.4.0.512           |DONE      |Manifest: 31:e6:db:63:47:4a:6e:e0:0a:2c:11:d1:76:db:4e:82:ff:56:2d:29:93:d2:e5:02:bd:d3:bd:9d:27:47:a5:71
		cataclysm_ut-7 - 1.20.1.jar                       |Cataclysm Apotheosis          |cataclysm_ut                  |1.7.0               |DONE      |Manifest: NOSIGNATURE
		arsmagicalegacy-1.20.1-1.4.0.jar                  |Ars Magica: Legacy            |arsmagicalegacy               |1.20.1-1.4.0        |DONE      |Manifest: NOSIGNATURE
		Apothic Supplementaries - Enchanting - 0.1.2a.jar |Apothic Supplementaries - Ench|apothic_sups_enchanting       |0.1.2               |DONE      |Manifest: NOSIGNATURE
		sliceanddice-forge-3.2.0.jar                      |Create Slice & Dice           |sliceanddice                  |3.2.0               |DONE      |Manifest: NOSIGNATURE
		mcw-lights-1.0.6-mc1.20.1forge.jar                |Macaw's Lights and Lamps      |mcwlights                     |1.0.6               |DONE      |Manifest: NOSIGNATURE
		YungsBetterJungleTemples-1.20-Forge-2.0.5.jar     |YUNG's Better Jungle Temples  |betterjungletemples           |1.20-Forge-2.0.5    |DONE      |Manifest: NOSIGNATURE
		elytraslot-forge-6.4.0+1.20.1.jar                 |Elytra Slot                   |elytraslot                    |6.4.0+1.20.1        |DONE      |Manifest: NOSIGNATURE
		mowziesmobs-1.6.5.jar                             |Mowzie's Mobs                 |mowziesmobs                   |1.6.4               |DONE      |Manifest: NOSIGNATURE
		doubledoors-1.20.1-5.7.jar                        |Double Doors                  |doubledoors                   |5.7                 |DONE      |Manifest: NOSIGNATURE
		harvestwithease-1.20.1-8.0.1.0-forge.jar          |Harvest with ease             |harvestwithease               |8.0.1.0             |DONE      |Manifest: NOSIGNATURE
		jei-1.20.1-forge-15.3.0.8.jar                     |Just Enough Items             |jei                           |15.3.0.8            |DONE      |Manifest: NOSIGNATURE
		VisualWorkbench-v8.0.0-1.20.1-Forge.jar           |Visual Workbench              |visualworkbench               |8.0.0               |DONE      |Manifest: 9a:09:85:98:65:c4:8c:11:c5:49:f6:d6:33:23:39:df:8d:b4:ff:92:84:b8:bd:a5:83:9f:ac:7f:2a:d1:4b:6a
		Pehkui-3.8.2+1.20.1-forge.jar                     |Pehkui                        |pehkui                        |3.8.2+1.20.1-forge  |DONE      |Manifest: NOSIGNATURE
		libraryferret-forge-1.20.1-4.0.0.jar              |Library ferret                |libraryferret                 |4.0.0               |DONE      |Manifest: NOSIGNATURE
		goblintraders-forge-1.20.1-1.9.3.jar              |Goblin Traders                |goblintraders                 |1.9.3               |DONE      |Manifest: 0d:78:5f:44:c0:47:0c:8c:e2:63:a3:04:43:d4:12:7d:b0:7c:35:37:dc:40:b1:c1:98:ec:51:eb:3b:3c:45:99
		epicsamurai-0.0.44-1.20.1-neo.jar                 |Epic Samurai                  |epicsamurai                   |0.0.44-1.20.1-neo   |DONE      |Manifest: NOSIGNATURE
		Mekanism-1.20.1-10.4.8.43.jar                     |Mekanism                      |mekanism                      |10.4.8              |DONE      |Manifest: NOSIGNATURE
		caelus-forge-3.2.0+1.20.1.jar                     |Caelus API                    |caelus                        |3.2.0+1.20.1        |DONE      |Manifest: NOSIGNATURE
		bdlib-1.27.0.8-mc1.20.1.jar                       |BdLib                         |bdlib                         |1.27.0.8            |DONE      |Manifest: NOSIGNATURE
		EpicFight-20.7.4.jar                              |Epic Fight                    |epicfight                     |20.7.4              |DONE      |Manifest: NOSIGNATURE
		refm-0.1.5-1.20.1.jar                             |Rapier For EpicFightMod       |refm                          |0.1-1.20.1          |DONE      |Manifest: NOSIGNATURE
		WeaponsOfMiracles-20.1.7.40.jar                   |Weapons of Minecraft          |wom                           |20.1.7.40           |DONE      |Manifest: NOSIGNATURE
		integrated_api-1.5.1+1.20.1-forge.jar             |Integrated API                |integrated_api                |1.5.1+1.20.1-forge  |DONE      |Manifest: NOSIGNATURE
		NaturesCompass-1.20.1-1.11.2-forge.jar            |Nature's Compass              |naturescompass                |1.20.1-1.11.2-forge |DONE      |Manifest: NOSIGNATURE
		EpheroLib-1.20.1-FORGE-1.2.0.jar                  |BOZOID                        |epherolib                     |0.1.2               |DONE      |Manifest: NOSIGNATURE
		neruina-forge-2.0.0-beta.10+1.20.1.jar            |Neruina                       |neruina                       |2.0.0-beta.10       |DONE      |Manifest: NOSIGNATURE
		fusion-1.1.1-forge-mc1.20.1.jar                   |Fusion                        |fusion                        |1.1.1               |DONE      |Manifest: NOSIGNATURE
		epictweaks-forge-1.20.1-1.0.1.jar                 |Epic Tweaks                   |epictweaks                    |1.0.1               |DONE      |Manifest: NOSIGNATURE
		ExtraDisks-1.20.1-3.0.2.jar                       |Extra Disks                   |extradisks                    |1.20.1-3.0.2        |DONE      |Manifest: NOSIGNATURE
		EdivadLib-1.20.1-2.0.1.jar                        |EdivadLib                     |edivadlib                     |2.0.1               |DONE      |Manifest: NOSIGNATURE
		puzzlesaccessapi-forge-8.0.7.jar                  |Puzzles Access Api            |puzzlesaccessapi              |8.0.7               |DONE      |Manifest: 9a:09:85:98:65:c4:8c:11:c5:49:f6:d6:33:23:39:df:8d:b4:ff:92:84:b8:bd:a5:83:9f:ac:7f:2a:d1:4b:6a
		forge-1.20.1-47.3.0-universal.jar                 |Forge                         |forge                         |47.3.0              |DONE      |Manifest: 84:ce:76:e8:45:35:e4:0e:63:86:df:47:59:80:0f:67:6c:c1:5f:6e:5f:4d:b3:54:47:1a:9f:7f:ed:5e:f2:90
		ironchest-1.20.1-14.4.4.jar                       |Iron Chests                   |ironchest                     |1.20.1-14.4.4       |DONE      |Manifest: NOSIGNATURE
		DungeonsArise-1.20.x-2.1.58-release.jar           |When Dungeons Arise           |dungeons_arise                |2.1.58-1.20.x       |DONE      |Manifest: NOSIGNATURE
		ZeroCore2-1.20.1-2.1.44.jar                       |Zero CORE 2                   |zerocore                      |1.20.1-2.1.44       |DONE      |Manifest: NOSIGNATURE
		client-1.20.1-20230612.114412-srg.jar             |Minecraft                     |minecraft                     |1.20.1              |DONE      |Manifest: a1:d4:5e:04:4f:d3:d6:e0:7b:37:97:cf:77:b0:de:ad:4a:47:ce:8c:96:49:5f:0a:cf:8c:ae:b2:6d:4b:8a:3f
		cofh_core-1.20.1-11.0.2.56.jar                    |CoFH Core                     |cofh_core                     |11.0.2              |DONE      |Manifest: NOSIGNATURE
		thermal_core-1.20.1-11.0.5.23.jar                 |Thermal Series                |thermal                       |11.0.5              |DONE      |Manifest: NOSIGNATURE
		thermal_integration-1.20.1-11.0.1.27.jar          |Thermal Integration           |thermal_integration           |11.0.1              |DONE      |Manifest: NOSIGNATURE
		thermal_innovation-1.20.1-11.0.1.23.jar           |Thermal Innovation            |thermal_innovation            |11.0.1              |DONE      |Manifest: NOSIGNATURE
		thermal_foundation-1.20.1-11.0.5.69.jar           |Thermal Foundation            |thermal_foundation            |11.0.5              |DONE      |Manifest: NOSIGNATURE
		thermal_locomotion-1.20.1-11.0.1.19.jar           |Thermal Locomotion            |thermal_locomotion            |11.0.1              |DONE      |Manifest: NOSIGNATURE
		thermal_dynamics-1.20.1-11.0.1.23.jar             |Thermal Dynamics              |thermal_dynamics              |11.0.1              |DONE      |Manifest: NOSIGNATURE
		smoothchunk-1.20.1-3.6.jar                        |Smoothchunk mod               |smoothchunk                   |1.20.1-3.6          |DONE      |Manifest: NOSIGNATURE
		voicechat-forge-1.20.1-2.5.17.jar                 |Simple Voice Chat             |voicechat                     |1.20.1-2.5.17       |DONE      |Manifest: NOSIGNATURE
		AdLods-1.20.1-8.1.2.0-build.0424.jar              |Large Ore Deposits            |adlods                        |8.1.2.0             |DONE      |Manifest: NOSIGNATURE
		spectrelib-forge-0.13.15+1.20.1.jar               |SpectreLib                    |spectrelib                    |0.13.15+1.20.1      |DONE      |Manifest: NOSIGNATURE
		domum_ornamentum-1.20.1-1.0.186-RELEASE-universal.|Domum Ornamentum              |domum_ornamentum              |1.20.1-1.0.186-RELEA|DONE      |Manifest: NOSIGNATURE
		kffmod-4.11.0.jar                                 |Kotlin For Forge              |kotlinforforge                |4.11.0              |DONE      |Manifest: NOSIGNATURE
		pipez-forge-1.20.1-1.2.12.jar                     |Pipez                         |pipez                         |1.20.1-1.2.12       |DONE      |Manifest: NOSIGNATURE
		notenoughanimations-forge-1.7.4-mc1.20.1.jar      |NotEnoughAnimations           |notenoughanimations           |1.7.4               |DONE      |Manifest: NOSIGNATURE
		flywheel-forge-1.20.1-0.6.10-7.jar                |Flywheel                      |flywheel                      |0.6.10-7            |DONE      |Manifest: NOSIGNATURE
		createoreexcavation-1.20-1.4.4.jar                |Create Ore Excavation         |createoreexcavation           |1.4.4               |DONE      |Manifest: NOSIGNATURE
		souls_like_universe_mod_20.1.810.jar              |souls like universe           |soulslikeuniverse             |20.1.810            |DONE      |Manifest: NOSIGNATURE
		itemcollectors-1.1.10-forge-mc1.20.jar            |Item Collectors               |itemcollectors                |1.1.10              |DONE      |Manifest: NOSIGNATURE
		Croptopia-1.20.1-FORGE-3.0.4.jar                  |Croptopia                     |croptopia                     |3.0.4               |DONE      |Manifest: NOSIGNATURE
		thermal_cultivation-1.20.1-11.0.1.24.jar          |Thermal Cultivation           |thermal_cultivation           |11.0.1              |DONE      |Manifest: NOSIGNATURE
		polymorph-forge-0.49.5+1.20.1.jar                 |Polymorph                     |polymorph                     |0.49.5+1.20.1       |DONE      |Manifest: NOSIGNATURE
		JustEnoughProfessions-forge-1.20.1-3.0.1.jar      |Just Enough Professions (JEP) |justenoughprofessions         |3.0.1               |DONE      |Manifest: NOSIGNATURE
		[1.20.1] SecurityCraft v1.9.10.jar                |SecurityCraft                 |securitycraft                 |1.9.10              |DONE      |Manifest: NOSIGNATURE
		Zeta-1.0-19.jar                                   |Zeta                          |zeta                          |1.0-19              |DONE      |Manifest: NOSIGNATURE
		structurize-1.20.1-1.0.733-RELEASE.jar            |Structurize                   |structurize                   |1.20.1-1.0.733-RELEA|DONE      |Manifest: NOSIGNATURE
		oceansdelight-1.0.2-1.20.jar                      |Ocean's Delight               |oceansdelight                 |1.0.2-1.20          |DONE      |Manifest: NOSIGNATURE
		appleskin-forge-mc1.20.1-2.5.1.jar                |AppleSkin                     |appleskin                     |2.5.1+mc1.20.1      |DONE      |Manifest: NOSIGNATURE
		moremobvariants-forge+1.20.1-1.3.0.1.jar          |More Mob Variants             |moremobvariants               |1.3.0.1             |DONE      |Manifest: NOSIGNATURE
		lootr-forge-1.20-0.7.34.86.jar                    |Lootr                         |lootr                         |0.7.34.85           |DONE      |Manifest: NOSIGNATURE
		connectedglass-1.1.11-forge-mc1.20.1.jar          |Connected Glass               |connectedglass                |1.1.11              |DONE      |Manifest: NOSIGNATURE
		PuzzlesLib-v8.1.20-1.20.1-Forge.jar               |Puzzles Lib                   |puzzleslib                    |8.1.20              |DONE      |Manifest: 9a:09:85:98:65:c4:8c:11:c5:49:f6:d6:33:23:39:df:8d:b4:ff:92:84:b8:bd:a5:83:9f:ac:7f:2a:d1:4b:6a
		Aquaculture-1.20.1-2.5.1.jar                      |Aquaculture 2                 |aquaculture                   |2.5.1               |DONE      |Manifest: NOSIGNATURE
		EFMCompat 2.0.jar                                 |EFM & Other Mods Weapons Compa|efm_compat                    |2.0                 |DONE      |Manifest: NOSIGNATURE
		cosmeticarmorreworked-1.20.1-v1a.jar              |CosmeticArmorReworked         |cosmeticarmorreworked         |1.20.1-v1a          |DONE      |Manifest: 5e:ed:25:99:e4:44:14:c0:dd:89:c1:a9:4c:10:b5:0d:e4:b1:52:50:45:82:13:d8:d0:32:89:67:56:57:01:53
		chunksending-1.20.1-2.8.jar                       |chunksending mod              |chunksending                  |1.20.1-2.8          |DONE      |Manifest: NOSIGNATURE
		aquamirae-6.API15.jar                             |Aquamirae                     |aquamirae                     |6.API15             |DONE      |Manifest: NOSIGNATURE
		cristellib-1.1.5-forge.jar                        |Cristel Lib                   |cristellib                    |1.1.5               |DONE      |Manifest: NOSIGNATURE
		ad_astra-forge-1.20.1-1.15.5.jar                  |Ad Astra                      |ad_astra                      |1.15.5              |DONE      |Manifest: NOSIGNATURE
		rsrequestify-1.20.1-2.3.3.jar                     |RSRequestify                  |rsrequestify                  |2.3.3               |DONE      |Manifest: NOSIGNATURE
		weaponmaster_ydm-forge-1.20.1-4.2.3.jar           |YDM's Weapon Master           |weaponmaster_ydm              |4.2.3               |DONE      |Manifest: NOSIGNATURE
		effs-1.0.0.jar                                    |EpicFightingStyles            |effs                          |1.0.0               |DONE      |Manifest: NOSIGNATURE
		SkyVillages-1.0.4-1.19.2-1.20.1-forge-release.jar |Sky Villages                  |skyvillages                   |1.0.4               |DONE      |Manifest: NOSIGNATURE
		kuma-api-forge-20.1.6+1.20.1.jar                  |KumaAPI                       |kuma_api                      |20.1.6              |DONE      |Manifest: NOSIGNATURE
		YungsBetterWitchHuts-1.20-Forge-3.0.3.jar         |YUNG's Better Witch Huts      |betterwitchhuts               |1.20-Forge-3.0.3    |DONE      |Manifest: NOSIGNATURE
		geckolib-forge-1.20.1-4.4.6.jar                   |GeckoLib 4                    |geckolib                      |4.4.6               |DONE      |Manifest: NOSIGNATURE
		ars_nouveau-1.20.1-4.12.1-all.jar                 |Ars Nouveau                   |ars_nouveau                   |4.12.1              |DONE      |Manifest: NOSIGNATURE
		ec_ars_plugin-1.20.1-1.0.3-all.jar                |Ars Expanded Combat           |ec_ars_plugin                 |1.0.3               |DONE      |Manifest: NOSIGNATURE
		shifu_epic_fight_skill_recipe-1.0.0-forge-1.20.1.j|Shifu Epic Fight Skill Recipe |shifu_epic_fight_skill_recipe |1.0.0               |DONE      |Manifest: NOSIGNATURE
		knightsnmages-0.0.7-neo.jar                       |KnightsnMages                 |knightsnmages                 |0.0.7-neo           |DONE      |Manifest: NOSIGNATURE
		IllagerInvasion-v8.0.5-1.20.1-Forge.jar           |Illager Invasion              |illagerinvasion               |8.0.5               |DONE      |Manifest: 9a:09:85:98:65:c4:8c:11:c5:49:f6:d6:33:23:39:df:8d:b4:ff:92:84:b8:bd:a5:83:9f:ac:7f:2a:d1:4b:6a
		YungsBetterOceanMonuments-1.20-Forge-3.0.4.jar    |YUNG's Better Ocean Monuments |betteroceanmonuments          |1.20-Forge-3.0.4    |DONE      |Manifest: NOSIGNATURE
		connectivity-1.20.1-5.5.jar                       |Connectivity Mod              |connectivity                  |1.20.1-5.5          |DONE      |Manifest: NOSIGNATURE
		sophisticatedcore-1.20.1-0.6.22.611.jar           |Sophisticated Core            |sophisticatedcore             |0.6.22.611          |DONE      |Manifest: NOSIGNATURE
		gpumemleakfix-1.20.1-1.8.jar                      |Gpu memory leak fix           |gpumemleakfix                 |1.20.1-1.8          |DONE      |Manifest: NOSIGNATURE
		InsaneLib-1.13.5-mc1.20.1.jar                     |InsaneLib                     |insanelib                     |1.13.5              |DONE      |Manifest: NOSIGNATURE
		cookingforblockheads-forge-1.20.1-16.0.6.jar      |CookingForBlockheads          |cookingforblockheads          |16.0.6              |DONE      |Manifest: NOSIGNATURE
		Controlling-forge-1.20.1-12.0.2.jar               |Controlling                   |controlling                   |12.0.2              |DONE      |Manifest: NOSIGNATURE
		Prism-1.20.1-forge-1.0.5.jar                      |Prism                         |prism                         |1.0.5               |DONE      |Manifest: NOSIGNATURE
		Placebo-1.20.1-8.6.2.jar                          |Placebo                       |placebo                       |8.6.2               |DONE      |Manifest: NOSIGNATURE
		citadel-2.5.4-1.20.1.jar                          |Citadel                       |citadel                       |2.5.4               |DONE      |Manifest: NOSIGNATURE
		alexsmobs-1.22.8.jar                              |Alex's Mobs                   |alexsmobs                     |1.22.8              |DONE      |Manifest: NOSIGNATURE
		iceandfire-2.1.13-1.20.1-beta-4.jar               |Ice and Fire                  |iceandfire                    |2.1.13-1.20.1-beta-4|DONE      |Manifest: NOSIGNATURE
		mixinextras-forge-0.2.0.jar                       |MixinExtras                   |mixinextras                   |0.2.0               |DONE      |Manifest: NOSIGNATURE
		ec_es_plugin-1.20.1-1.1.2-all.jar                 |EC Epic Samurais Plugin       |ec_es_plugin                  |1.1.2               |DONE      |Manifest: NOSIGNATURE
		expanded_combat-1.20.1-3.1.2-all.jar              |Expanded Combat               |expanded_combat               |3.1.2               |DONE      |Manifest: NOSIGNATURE
		ec_ef_plugin-1.20.1-1.2.3-all.jar                 |EC Epic Fight Compat          |ec_ef_plugin                  |1.2.3               |DONE      |Manifest: NOSIGNATURE
		Bookshelf-Forge-1.20.1-20.2.13.jar                |Bookshelf                     |bookshelf                     |20.2.13             |DONE      |Manifest: eb:c4:b1:67:8b:f9:0c:db:dc:4f:01:b1:8e:61:64:39:4c:10:85:0b:a6:c4:c7:48:f0:fa:95:f2:cb:08:3a:e5
		sophisticatedbackpacks-1.20.1-3.20.5.1044.jar     |Sophisticated Backpacks       |sophisticatedbackpacks        |3.20.5.1044         |DONE      |Manifest: NOSIGNATURE
		create_dragon_lib-1.20.1-1.4.3.jar                |Create: Dragon Lib            |create_dragon_lib             |1.4.3               |DONE      |Manifest: NOSIGNATURE
		relics-1.20.1-0.6.5.2.jar                         |Relics                        |relics                        |0.6.5.2             |DONE      |Manifest: NOSIGNATURE
		Waddles-1.20.1-0.9.4.jar                          |Waddles                       |waddles                       |0.9.4               |DONE      |Manifest: NOSIGNATURE
		takesapillage-1.0.3-1.20.1.jar                    |It Takes A Pillage            |takesapillage                 |1.0.3               |DONE      |Manifest: NOSIGNATURE
		ProgressiveBosses-3.9.7-mc1.20.1.jar              |Progressive Bosses            |progressivebosses             |3.9.7-mc1.20.1      |DONE      |Manifest: NOSIGNATURE
		mcw-doors-1.1.1forge-mc1.20.1.jar                 |Macaw's Doors                 |mcwdoors                      |1.1.1               |DONE      |Manifest: NOSIGNATURE
		bygonenether-1.3.2-1.20.x.jar                     |Bygone Nether                 |bygonenether                  |1.3.2               |DONE      |Manifest: NOSIGNATURE
		Steam_Rails-1.6.4+forge-mc1.20.1.jar              |Create: Steam 'n' Rails       |railways                      |1.6.4+forge-mc1.20.1|DONE      |Manifest: NOSIGNATURE
		MekanismGenerators-1.20.1-10.4.8.43.jar           |Mekanism: Generators          |mekanismgenerators            |10.4.8              |DONE      |Manifest: NOSIGNATURE
		carryon-forge-1.20.1-2.1.2.7.jar                  |Carry On                      |carryon                       |2.1.2.7             |DONE      |Manifest: NOSIGNATURE
		ShieldExpansion-1.20.1-1.1.7a.jar                 |Shield Expansion              |shieldexp                     |1.1.7a              |DONE      |Manifest: NOSIGNATURE
		dummmmmmy-1.20-1.8.17b.jar                        |MmmMmmMmmmmm                  |dummmmmmy                     |1.20-1.8.17b        |DONE      |Manifest: NOSIGNATURE
		twilightforest-1.20.1-4.3.2145-universal.jar      |The Twilight Forest           |twilightforest                |4.3.2145            |DONE      |Manifest: NOSIGNATURE
		RSInfinityBooster-1.20.1-1.0+32.jar               |RSInfinityBooster             |rsinfinitybooster             |1.20.1-1.0+32       |DONE      |Manifest: NOSIGNATURE
		refinedstorage-1.12.4.jar                         |Refined Storage               |refinedstorage                |1.12.4              |DONE      |Manifest: NOSIGNATURE
		FarmersDelight-1.20.1-1.2.4.jar                   |Farmer's Delight              |farmersdelight                |1.20.1-1.2.4        |DONE      |Manifest: NOSIGNATURE
		ends_delight-1.20.1-1.0.1.jar                     |End's Delight                 |ends_delight                  |1.0.1               |DONE      |Manifest: NOSIGNATURE
		endersdelight-1.20.1-1.0.3.jar                    |Ender's Delight               |endersdelight                 |1.0.3               |DONE      |Manifest: NOSIGNATURE
		endrem_forge-5.2.3-R-1.20.X.jar                   |End Remastered                |endrem                        |5.2.3-R-1.20.1      |DONE      |Manifest: NOSIGNATURE
		mcw-fences-1.1.2-mc1.20.1forge.jar                |Macaw's Fences and Walls      |mcwfences                     |1.1.2               |DONE      |Manifest: NOSIGNATURE
		born_in_chaos_[Forge]1.20.1_1.3.1.jar             |Born in Chaos                 |born_in_chaos_v1              |1.0.0               |DONE      |Manifest: NOSIGNATURE
		lionfishapi-1.9.jar                               |LionfishAPI                   |lionfishapi                   |1.9                 |DONE      |Manifest: NOSIGNATURE
		dungeons_enhanced-1.20.1-5.2.2.jar                |Dungeons Enhanced             |dungeons_enhanced             |5.2.2               |DONE      |Manifest: NOSIGNATURE
		L_Enders_Cataclysm-1.99.5 -1.20.1.jar             |Cataclysm Mod                 |cataclysm                     |1.99.5              |DONE      |Manifest: NOSIGNATURE
		Patchouli-1.20.1-84-FORGE.jar                     |Patchouli                     |patchouli                     |1.20.1-84-FORGE     |DONE      |Manifest: NOSIGNATURE
		ars_additions-1.20.1-1.5.1.jar                    |Ars Additions                 |ars_additions                 |1.20.1-1.5.1        |DONE      |Manifest: NOSIGNATURE
		blockui-1.20.1-1.0.156-RELEASE.jar                |UI Library Mod                |blockui                       |1.20.1-1.0.156-RELEA|DONE      |Manifest: NOSIGNATURE
		multipiston-1.20-1.2.43-RELEASE.jar               |Multi-Piston                  |multipiston                   |1.20-1.2.43-RELEASE |DONE      |Manifest: NOSIGNATURE
		collective-1.20.1-7.61.jar                        |Collective                    |collective                    |7.61                |DONE      |Manifest: NOSIGNATURE
		CerbonsApi-Forge-1.20.1-1.0.0.jar                 |CerbonsApi                    |cerbons_api                   |1.0.0               |DONE      |Manifest: NOSIGNATURE
		villagertools-1.20.1-1.0.3.jar                    |villagertools                 |villagertools                 |1.0.3               |DONE      |Manifest: 1f:47:ac:b1:61:82:96:b8:47:19:16:d2:61:81:11:60:3a:06:4b:61:31:56:7d:44:31:1e:0c:6f:22:5b:4c:ed
		thermal_expansion-1.20.1-11.0.1.29.jar            |Thermal Expansion             |thermal_expansion             |11.0.1              |DONE      |Manifest: NOSIGNATURE
		BetterThirdPerson-Forge-1.20-1.9.0.jar            |Better Third Person           |betterthirdperson             |1.9.0               |DONE      |Manifest: NOSIGNATURE
		witherstormmod-1.20.1-4.1-all.jar                 |Cracker's Wither Storm Mod    |witherstormmod                |4.1                 |DONE      |Manifest: NOSIGNATURE
		ftb-ultimine-forge-2001.1.5.jar                   |FTB Ultimine                  |ftbultimine                   |2001.1.5            |DONE      |Manifest: NOSIGNATURE
		YungsBetterStrongholds-1.20-Forge-4.0.3.jar       |YUNG's Better Strongholds     |betterstrongholds             |1.20-Forge-4.0.3    |DONE      |Manifest: NOSIGNATURE
		resourcefullib-forge-1.20.1-2.1.25.jar            |Resourceful Lib               |resourcefullib                |2.1.25              |DONE      |Manifest: NOSIGNATURE
		MekanismTools-1.20.1-10.4.8.43.jar                |Mekanism: Tools               |mekanismtools                 |10.4.8              |DONE      |Manifest: NOSIGNATURE
		twilightdelight-2.0.11.jar                        |Twilight's Flavor & Delight   |twilightdelight               |2.0.11              |DONE      |Manifest: NOSIGNATURE
		SpartanWeaponry-1.20.1-forge-3.1.0-beta-1-all.jar |Spartan Weaponry              |spartanweaponry               |3.1.0-beta-1        |DONE      |Manifest: NOSIGNATURE
		architectury-9.2.14-forge.jar                     |Architectury                  |architectury                  |9.2.14              |DONE      |Manifest: NOSIGNATURE
		letsdo-API-forge-1.2.13-forge.jar                 |[Let's Do] API                |doapi                         |1.2.13              |DONE      |Manifest: NOSIGNATURE
		ftb-library-forge-2001.2.2.jar                    |FTB Library                   |ftblibrary                    |2001.2.2            |DONE      |Manifest: NOSIGNATURE
		ftb-teams-forge-2001.3.0.jar                      |FTB Teams                     |ftbteams                      |2001.3.0            |DONE      |Manifest: NOSIGNATURE
		letsdo-brewery-forge-1.1.9.jar                    |[Let's Do] Brewery            |brewery                       |1.1.9               |DONE      |Manifest: NOSIGNATURE
		yuushya-1.20.1-forge-2.1.1.jar                    |Yuushya                       |yuushya                       |2.1.1               |DONE      |Manifest: NOSIGNATURE
		cupboard-1.20.1-2.6.jar                           |Cupboard utilities            |cupboard                      |1.20.1-2.6          |DONE      |Manifest: NOSIGNATURE
		ExtremeReactors2-1.20.1-2.0.80.jar                |Extreme Reactors              |bigreactors                   |1.20.1-2.0.80       |DONE      |Manifest: NOSIGNATURE
		framework-forge-1.20.1-0.7.6.jar                  |Framework                     |framework                     |0.7.6               |DONE      |Manifest: 0d:78:5f:44:c0:47:0c:8c:e2:63:a3:04:43:d4:12:7d:b0:7c:35:37:dc:40:b1:c1:98:ec:51:eb:3b:3c:45:99
		smallships-forge-1.20.1-2.0.0-b1.3.jar            |Small Ships                   |smallships                    |2.0.0-b1.3          |DONE      |Manifest: NOSIGNATURE
		Towns-and-Towers-1.12-Fabric+Forge.jar            |Towns and Towers              |t_and_t                       |0.0NONE             |DONE      |Manifest: NOSIGNATURE
		Cucumber-1.20.1-7.0.8.jar                         |Cucumber Library              |cucumber                      |7.0.8               |DONE      |Manifest: NOSIGNATURE
		amendments-1.20-1.2.4.jar                         |Amendments                    |amendments                    |1.20-1.2.4          |DONE      |Manifest: NOSIGNATURE
		ars_extended_glyphs-1.20.1-1.8.jar                |Ars Nouveau - Extended Glyphs |ars_extended_glyphs           |1.20.1-1.8          |DONE      |Manifest: NOSIGNATURE
		sophisticatedstorage-1.20.1-0.10.25.804.jar       |Sophisticated Storage         |sophisticatedstorage          |0.10.25.804         |DONE      |Manifest: NOSIGNATURE
		octolib-1.20.1-0.3.jar                            |OctoLib                       |octolib                       |0.3                 |DONE      |Manifest: NOSIGNATURE
		the-conjurer-1.20.1-1.1.6.jar                     |The Conjurer                  |conjurer_illager              |1.1.6               |DONE      |Manifest: NOSIGNATURE
		obscure_api-15.jar                                |Obscure API                   |obscure_api                   |15                  |DONE      |Manifest: NOSIGNATURE
		create-1.20.1-0.5.1.f.jar                         |Create                        |create                        |0.5.1.f             |DONE      |Manifest: NOSIGNATURE
		Delightful-1.20.1-3.5.5.jar                       |Delightful                    |delightful                    |3.5.5               |DONE      |Manifest: NOSIGNATURE
		create_central_kitchen-1.20.1-for-create-0.5.1.f-1|Create: Central Kitchen       |create_central_kitchen        |1.3.12              |DONE      |Manifest: NOSIGNATURE
		ars_creo-1.20.1-4.1.0.jar                         |Ars Creo                      |ars_creo                      |4.1.0               |DONE      |Manifest: NOSIGNATURE
		waystones-forge-1.20-14.1.3.jar                   |Waystones                     |waystones                     |14.1.3              |DONE      |Manifest: NOSIGNATURE
		Structory_1.20.x_v1.3.5.jar                       |Structory                     |structory                     |1.3.5               |DONE      |Manifest: NOSIGNATURE
		mcw-paintings-1.0.5-1.20.1forge.jar               |Macaw's Paintings             |mcwpaintings                  |1.0.5               |DONE      |Manifest: NOSIGNATURE
		comforts-forge-6.3.5+1.20.1.jar                   |Comforts                      |comforts                      |6.3.5+1.20.1        |DONE      |Manifest: NOSIGNATURE
		artifacts-forge-9.5.11.jar                        |Artifacts                     |artifacts                     |9.5.11              |DONE      |Manifest: NOSIGNATURE
		crackerslib-forge-1.20.1-0.3.2.1.jar              |CrackersLib                   |crackerslib                   |1.20.1-0.3.2.1      |DONE      |Manifest: NOSIGNATURE
		decorative_blocks-forge-1.20.1-4.1.3.jar          |Decorative Blocks             |decorative_blocks             |4.1.3               |DONE      |Manifest: NOSIGNATURE
		[1.20.1-forge]-Epic-Knights-9.8.jar               |Epic Knights Mod              |magistuarmory                 |9.8                 |DONE      |Manifest: NOSIGNATURE
		[1.20.x-forge]-Epic-Knights-Addon-1.6.jar         |Epic Knights: Addon           |magistuarmoryaddon            |1.6                 |DONE      |Manifest: NOSIGNATURE
		Dungeon Crawl-1.20.1-2.3.14.jar                   |Dungeon Crawl                 |dungeoncrawl                  |2.3.14              |DONE      |Manifest: NOSIGNATURE
		mcjtylib-1.20-8.0.5.jar                           |McJtyLib                      |mcjtylib                      |1.20-8.0.5          |DONE      |Manifest: NOSIGNATURE
		rftoolsbase-1.20-5.0.4.jar                        |RFToolsBase                   |rftoolsbase                   |1.20-5.0.4          |DONE      |Manifest: NOSIGNATURE
		rftoolspower-1.20-6.0.2.jar                       |RFToolsPower                  |rftoolspower                  |1.20-6.0.2          |DONE      |Manifest: NOSIGNATURE
		YungsBetterDesertTemples-1.20-Forge-3.0.3.jar     |YUNG's Better Desert Temples  |betterdeserttemples           |1.20-Forge-3.0.3    |DONE      |Manifest: NOSIGNATURE
		ExplorersCompass-1.20.1-1.3.3-forge.jar           |Explorer's Compass            |explorerscompass              |1.20.1-1.3.3-forge  |DONE      |Manifest: NOSIGNATURE
		mahoutsukai-1.20.1-v1.34.62.jar                   |Mahou Tsukai                  |mahoutsukai                   |1.20.1-v1.34.62     |DONE      |Manifest: NOSIGNATURE
		BOMD-Forge-1.20.1-1.1.1.jar                       |Bosses of Mass Destruction    |bosses_of_mass_destruction    |1.1.1               |DONE      |Manifest: NOSIGNATURE
		azurelib-neo-1.20.1-2.0.26.jar                    |AzureLib                      |azurelib                      |2.0.26              |DONE      |Manifest: NOSIGNATURE
		EnderStorage-1.20.1-2.11.0.188-universal.jar      |EnderStorage                  |enderstorage                  |2.11.0.188          |DONE      |Manifest: 31:e6:db:63:47:4a:6e:e0:0a:2c:11:d1:76:db:4e:82:ff:56:2d:29:93:d2:e5:02:bd:d3:bd:9d:27:47:a5:71
		watut-forge-1.20.1-1.1.1.jar                      |What Are They Up To           |watut                         |1.20.1-1.1.1        |DONE      |Manifest: NOSIGNATURE
		ftb-chunks-forge-2001.3.1.jar                     |FTB Chunks                    |ftbchunks                     |2001.3.1            |DONE      |Manifest: NOSIGNATURE
		BrandonsCore-1.20.1-3.2.1.302-universal.jar       |Brandon's Core                |brandonscore                  |3.2.1.302           |DONE      |Manifest: 53:bb:a0:11:bd:61:e2:1a:e2:cb:fd:f8:4f:e4:cd:a5:cc:12:f4:43:f0:78:68:3b:e1:62:c6:78:3b:27:ff:fe
		Draconic-Evolution-1.20.1-3.1.2.575-universal.jar |Draconic Evolution            |draconicevolution             |3.1.2.575           |DONE      |Manifest: 53:bb:a0:11:bd:61:e2:1a:e2:cb:fd:f8:4f:e4:cd:a5:cc:12:f4:43:f0:78:68:3b:e1:62:c6:78:3b:27:ff:fe
		friendsandfoes-forge-mc1.20.1-2.0.10.jar          |Friends&Foes                  |friendsandfoes                |2.0.10              |DONE      |Manifest: NOSIGNATURE
		MysticalAgriculture-1.20.1-7.0.11.jar             |Mystical Agriculture          |mysticalagriculture           |7.0.11              |DONE      |Manifest: NOSIGNATURE
		MysticalAgradditions-1.20.1-7.0.3.jar             |Mystical Agradditions         |mysticalagradditions          |7.0.3               |DONE      |Manifest: NOSIGNATURE
		ars_trinkets-1.20.1-3.0.1.jar                     |Ars Nouveau Trinkets          |ars_trinkets                  |1.20.1-3.0.1        |DONE      |Manifest: NOSIGNATURE
		moonlight-1.20-2.11.41-forge.jar                  |Moonlight Library             |moonlight                     |1.20-2.11.41        |DONE      |Manifest: NOSIGNATURE
		titanium-1.20.1-3.8.28.jar                        |Titanium                      |titanium                      |3.8.28              |DONE      |Manifest: NOSIGNATURE
		mysterious_mountain_lib-1.4.7-1.20.1.jar          |Mysterious Mountain Lib       |mysterious_mountain_lib       |1.4.7-1.20.1        |DONE      |Manifest: NOSIGNATURE
		corn_delight-1.0.4-1.20.1.jar                     |Corn Delight                  |corn_delight                  |1.0.4-1.20.1        |DONE      |Manifest: NOSIGNATURE
		mixinsquared-forge-0.1.1.jar                      |MixinSquared                  |mixinsquared                  |0.1.1               |DONE      |Manifest: NOSIGNATURE
		Jade-1.20.1-forge-11.9.2.jar                      |Jade                          |jade                          |11.9.2+forge        |DONE      |Manifest: NOSIGNATURE
		forbidden_arcanus-1.20.1-2.2.6.jar                |Forbidden & Arcanus           |forbidden_arcanus             |1.20.1-2.2.6        |DONE      |Manifest: NOSIGNATURE
		nethersdelight-1.20.1-4.0.jar                     |Nether's Delight              |nethersdelight                |1.20.1-4.0          |DONE      |Manifest: NOSIGNATURE
		easy_villagers-1.20.1-1.0.17.jar                  |Easy Villagers                |easy_villagers                |1.20.1-1.0.17       |DONE      |Manifest: NOSIGNATURE
		Iceberg-1.20.1-forge-1.1.21.jar                   |Iceberg                       |iceberg                       |1.1.21              |DONE      |Manifest: NOSIGNATURE
		LegendaryTooltips-1.20.1-forge-1.4.5.jar          |Legendary Tooltips            |legendarytooltips             |1.4.5               |DONE      |Manifest: NOSIGNATURE
		brutalbosses-1.20.1-7.0.jar                       |brutalbosses mod              |brutalbosses                  |1.20.1-7.0          |DONE      |Manifest: NOSIGNATURE
		create-stuff-additions1.20.1_v2.0.4a.jar          |Create Stuff & Additions      |create_sa                     |2.0.4.              |DONE      |Manifest: NOSIGNATURE
		storagedrawers-1.20.1-12.0.3.jar                  |Storage Drawers               |storagedrawers                |12.0.3              |DONE      |Manifest: NOSIGNATURE
		FluxNetworks-1.20.1-7.2.1.15.jar                  |Flux Networks                 |fluxnetworks                  |7.2.1.15            |DONE      |Manifest: NOSIGNATURE
		ars_elemental-1.20.1-0.6.5.jar                    |Ars Elemental                 |ars_elemental                 |1.20.1-0.6.5        |DONE      |Manifest: NOSIGNATURE
		irons_spellbooks-1.20.1-3.1.7.1.jar               |Iron's Spells 'n Spellbooks   |irons_spellbooks              |1.20.1-3.1.7.1      |DONE      |Manifest: NOSIGNATURE
		additional_attributes-1.20.1-1.0.3-all.jar        |Additional Attributes         |additional_attributes         |1.0.3               |DONE      |Manifest: NOSIGNATURE
		betterchunkloading-1.20.1-4.3.jar                 |betterchunkloading mod        |betterchunkloading            |1.20.1-4.3          |DONE      |Manifest: NOSIGNATURE
		coroutil-forge-1.20.1-1.3.7.jar                   |CoroUtil                      |coroutil                      |1.20.1-1.3.7        |DONE      |Manifest: NOSIGNATURE
		epic_fight_battle_styles-1.1.5-1.20.1.jar         |Epic Fight Battle Styles      |epic_fight_battle_styles      |1.1.4               |DONE      |Manifest: NOSIGNATURE
		alexsdelight-1.5.jar                              |Alex's Delight                |alexsdelight                  |1.5                 |DONE      |Manifest: NOSIGNATURE
		ferritecore-6.0.1-forge.jar                       |Ferrite Core                  |ferritecore                   |6.0.1               |DONE      |Manifest: 41:ce:50:66:d1:a0:05:ce:a1:0e:02:85:9b:46:64:e0:bf:2e:cf:60:30:9a:fe:0c:27:e0:63:66:9a:84:ce:8a
		solcarrot-1.20.1-1.15.1.jar                       |Spice of Life: Carrot Edition |solcarrot                     |1.15.1              |DONE      |Manifest: NOSIGNATURE
		functionalstorage-1.20.1-1.2.10.jar               |Functional Storage            |functionalstorage             |1.20.1-1.2.10       |DONE      |Manifest: NOSIGNATURE
		charmofundying-forge-6.5.0+1.20.1.jar             |Charm of Undying              |charmofundying                |6.5.0+1.20.1        |DONE      |Manifest: NOSIGNATURE
		refinedstorageaddons-0.10.0.jar                   |Refined Storage Addons        |refinedstorageaddons          |0.10.0              |DONE      |Manifest: NOSIGNATURE
		refinedpolymorph-0.1.1-1.20.1.jar                 |Refined Polymorphism          |refinedpolymorph              |0.1.1-1.20.1        |DONE      |Manifest: NOSIGNATURE
		CrabbersDelight-1.20.1-1.1.4a.jar                 |Crabber's Delight             |crabbersdelight               |1.1.4               |DONE      |Manifest: NOSIGNATURE
		packetfixer-forge-1.4.2-1.19-to-1.20.1.jar        |Packet Fixer                  |packetfixer                   |1.4.2               |DONE      |Manifest: NOSIGNATURE
		expandability-forge-9.0.4.jar                     |ExpandAbility                 |expandability                 |9.0.4               |DONE      |Manifest: NOSIGNATURE
		valhelsia_core-forge-1.20.1-1.1.2.jar             |Valhelsia Core                |valhelsia_core                |1.1.2               |DONE      |Manifest: NOSIGNATURE
		create_enchantment_industry-1.20.1-for-create-0.5.|Create Enchantment Industry   |create_enchantment_industry   |1.2.9.d             |DONE      |Manifest: NOSIGNATURE
		createaddition-1.20.1-1.2.3.jar                   |Create Crafts & Additions     |createaddition                |1.20.1-1.2.3        |DONE      |Manifest: NOSIGNATURE
	Crash Report UUID: aab13b50-91cb-4cfc-adb6-644d5814968a
	FML: 47.3
	Forge: net.minecraftforge:47.3.0
	Flywheel Backend: GL33 Instanced Arrays
