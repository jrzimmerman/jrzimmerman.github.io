+++
author = "Justin Zimmerman"
date = "2015-12-06T09:05:42-04:00"
description = "Seamless is an image resizing application that leverages Firebase for persistent storage of a users images."
draft = true
keywords = ["Seamless", "Seam Carving", "Seam", "Carving", "Hack Reactor", "Hack", "Reactor"]
tags = ["Seamless", "Hack Reactor"]
title = "Seamless"
topics = ["Seamless"]
type = "post"

+++

[Seamless](https://hrr9-seamless.herokuapp.com/) is an image resizing application that leverages [Firebase](https://www.firebase.com/) for persistent storage of a users images.

The name Seamless is derived from the [seam carving](https://en.wikipedia.org/wiki/Seam_carving) algorithm it uses for image resizing. The seam carving algorithm iterates over each pixel, and generates an energy value. The energy values are measured by the pixel's contrast to other surrounding pixels.

After the energy values are calculated, the algorithm will create a "seam" through the image, finding the lowest energy values either top to bottom, or left to right. Once the seam is cut multiple times to fit the intended size, the process is complete.

After the algorithm has completed, the application allows users to either save their changes to Firebase, or revert back to the original image.

Also included with our application is a gallery, that holds all of the user's previously saved images.

This project was a very rewarding experience, and I really enjoyed working with my group to complete the application. 
 