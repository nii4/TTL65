# Description
A simple Magisk module to add a setting of TTL=65, for tethering. With the Magisk module, the system setting change will be applied on reboots and after updates. No more need for commands, terminals or scripts. This is meant to be used on devices which are connecting to your mobile hotspot. 

# Install
Download the latest release and flash with Magisk.

# Usage
Flash and forget. Your TTL should now be set to 65 even after reboots and updates.

If you want to check the TTL setting for yourself, you can do so in the following way:

1. Open a terminal on your device (ex - Termux)
2. Grant root access
    ```bash
    su
    ```
3. Check TTL
    ```bash
    cat /proc/sys/net/ipv4/ip_default_ttl
    ```

Alternatively, you can open a file explorer with root access and navigate to the ``ip_default_ttl`` file at:
```
/proc/sys/net/ipv4/ip_default_ttl
```
