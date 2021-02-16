---
title: Manifest and Main Class
---

# Manifest and Main Class


```java
package org.mcnative.example;

import net.pretronic.libraries.plugin.lifecycle.Lifecycle;
import net.pretronic.libraries.plugin.lifecycle.LifecycleState;
import org.mcnative.common.plugin.MinecraftPlugin;

public class McNativeExamplePlugin extends MinecraftPlugin {

    @Lifecycle(state = LifecycleState.BOOTSTRAP)
    public void onLoad(LifecycleState state){
        getLogger().info("My plugin started successfully");
    }


    @Lifecycle(state = LifecycleState.SHUTDOWN)
    public void onShutdown(LifecycleState state){
        getLogger().info("My plugin stopped successfully");
    }

}
```
