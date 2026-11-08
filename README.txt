AutoJoin (1.21.11 Fabric, client-side)

Build:  copy the gradle/ folder + gradlew + gradlew.bat from one of your other mod projects into this folder, then:
        ./gradlew build     ->  build/libs/autojoin-1.0.0.jar  (put in .minecraft/mods with Fabric API)

Use:    Free For All -> Map Selection -> hover the map you want -> press J.
        It clicks the map; on "This game is currently full!" it clicks Back, reopens Map Selection, re-clicks the same map.
        Press J again to stop. It auto-stops when the menu closes (you got in) or you disconnect.

Tuning:  AutoJoinClient.java top constants: TOGGLE_KEY, RETRY_TICKS (lower = faster re-click), NO_SCREEN_STOP_TICKS.

Queue handling (from your clip): when a spot opens the server says "Queueing for Specific Game", gives you a "Leave Queue" hotbar item and keeps the
menu open. The mod now stops clicking while queued and waits for "Game found!". Press J again to stop the mod entirely.
