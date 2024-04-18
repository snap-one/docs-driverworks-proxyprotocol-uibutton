## supports\_color

Whether the device can show a broad range of colors.  Set to False and use "supports\_color\_predefined" if the driver can only reproduce a limited number of colors, such as devices that only use enums to communicate or hardware with a limited table of factory configured colors.

### Signature

`<supports_color></supports_color>`


### Type

Boolean: Defaults to false.

### Dynamic Capability

Yes

### Example

```xml
<capabilities>
    <supports_color>false</supports_color>
</capabilities>
```


### Usage Note

If changing the supports\_color or supports\_color\_correlated\_temperature capabilities via the Dynamic Capabilities Notify, these should both be done in a single notification. If only one is disabled/enabled at a time, device color presets such as the On or Dim colors may have their color mode changed between Full Color and CCT automatically.

For example,  if the presets mode were CCT and a driver on director startup dynamically enabled just supports\_color the proxy would detect that CCT is not supported and change any existing presets to color mode Full Color.