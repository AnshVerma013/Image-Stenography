# Image-Stenography

Alright, so LSB steganography, it's a pretty neat concept in the realm of covert communication. LSB, or Least Significant Bit, is all about flying under the radar, you know? The idea is to tweak the least significant bit of a pixel's color value, because let's face it, altering that tiny detail won't raise too many eyebrows.

Picture this: you've got your image, right? Each pixel's got its RGB values, plus an alpha channel for opacity. Now, what if we sneakily stash away data in those last two bits of each channel? That's like having a secret compartment in every pixel, perfect for hiding messages. I'm talking one character per pixel, folks. Talk about discreet.

So, here's the drill for hiding data. First off, we need to prep our canvas, making sure those last two bits are clear for our covert ops. Then, we add a little tag at the beginning of our message, like "valid," just to mark the starting line. After converting our sneaky message into binary, it's just a matter of slipping those bits into the pixel channels. Smooth, right?

Now, extracting the goods is a whole other game. We grab our image, peek into those last two bits of each pixel, and decode them back into good old ASCII characters. And hey, remember that "valid" tag? It's like our secret handshake. If it's missing, we know the image's clean as a whistle.

But wait, what if someone tries to extract from an innocent image? No worries, our trusty "valid" tag comes to the rescue again. If it's not there, we know there's no hidden treasure to find.

See, LSB steganography is like being a cyber-spy, sneaking messages right under everyone's noses. It's the stuff of covert legends, my friends.

Go nuts~
