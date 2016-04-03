# Mangrove
Javascript Utilites Pack

Pubstick  --> Utility to pub-sub type message delivery system on web workers.

Pub Sub is a well known pattern for communication among loosely related components in the javascript world. Since javascript has been traditionally single threaded, this pattern is conventionally implemented as a global store of callbacks stored in a dictionary and executed one after the other.The major pain point in working with web workers is that they don't gel seamlessly with your existing javascript code for the following reasons:
 -> Web workers do not acknowledge the existing functions which you may be needed in the code which is run async.
 -> Passing back computation results to the paretn thread does not follow promise type patterns.
 -> Inability to send context to web workers in form module deependencies.
 -> General patterns like map-filter-aggregate have to be implemented from scratch everytime.

