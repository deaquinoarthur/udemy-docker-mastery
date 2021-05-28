# Docker Mastery

**Topics**

- All about images, the building block of containers
- What is an image, and what it isn't
- Using docker hub registry
- Managing our local image cache
- Building our own images

## What's In An Image and What Isn't

- App binaries and dependencies
- Metadata about the image data and how to run the image
- **Official definition:** "An image is an ordered collection of root
  filesystem changes and the corresponding execution parameters for use within a
  container runtime"
- Not a complete OS. No kernel, kernel modules (e.g. drivers), it's really just,
  the binaries that an application needs, because the host provides the kernel.
- An image can be:
  - Small as one file (your app binary) like a golang static binary
  - Big as Ubuntu distro with apt, and Apache, PHP, and more installed
