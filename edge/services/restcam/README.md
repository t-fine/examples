# Horizon Monitor Service

Restcam is a dependent service of the [Horizon object detection and classification example edge services](../visual_inferencing/README.md). The `visual_inferencing` examples are designed to make use of a camera, or a webcam. By default they try to use this `restcam` service and it, in turn, uses the popular [fswebcam](https://github.com/fsphil/fswebcam) software to view the world through your camera. If image retrieval fails (e.g., if you don't have a camera attached) the raw original of the image above (before inferencing, and without any bounding boxes, laebls, etc.) will be provided by the `restcam` service. The `restcam` service provides images in the form of an image file, suitable for embedding in an HTML document. So you can easily replace the `restcam` service with another image source anywhere on your LAN or even out on the Internet.