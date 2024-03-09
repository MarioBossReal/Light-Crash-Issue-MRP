# Light-Crash-Issue-MRP

Having many lights on screen in forward+ causes the editor to become fully non-funcitonal, requiring restart.

ERROR: Condition "err != VK_SUCCESS" is true. Returning: FAILED
   at: command_queue_execute_and_present (drivers/vulkan/rendering_device_driver_vulkan.cpp:2214)
ERROR: Unable to acquire framebuffer.
   at: (servers/rendering/rendering_device.cpp:3199)

This issue is 100% reproducable in Godot 4.3 dev 3, Godot 4.3 dev 4, and presumably in other 4.3 dev branches.
This issue does not occur at all on current stable branch (4.2.1).

# How to use this MRP

- Import the project into a Godot 4.3 editor.
- Open "light_crash.tscn"
- Pan the viewport camera around to the right

The editor will become non-functional.
