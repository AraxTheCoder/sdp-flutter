# SDP for Flutter - a scalable size unit
An Flutter SDK that provides a new size unit - sdp (scalable dp). This size unit scales with the screen size. It can help Flutter developers with supporting multiple screens.

Based on [sdp from intuit](https://github.com/intuit/sdp) but written for Flutter. 

# Attention
Use it carefully! for example, in most cases you still need to design a different layout for tablets.

# Example
![sdp example](https://github.com/intuit/sdp/blob/master/sdp_example.png)

And is the same layout built using dp:

![dp example](https://github.com/intuit/sdp/blob/master/dp_example.png)

You can see that sdp scales with the screen size and the dp stays with the same size on all screen sizes.

# Getting Started

To add sdp for Flutter to your project just add the SDP.dart file in an location of your choice.

To use it, run the init method right at the Widget build method:
  
```
@override
Widget build(BuildContext context) {
  SDP.init(context);
}
```

And to calculate the sdp size just call:

```
SDP.sdp(sizeInFlutterLP);
```

For easy mapping of designs to sdp units, one can create designs with 300 pixels screen width - in this case each pixel in the design corresponds to 1 sdp.

# Note
Unlike the library for android, this one adjusts the sdp size unit to the width of the display with pixel accuracy.

All rights of the screenshots belong to [Intuit](https://github.com/intuit)
