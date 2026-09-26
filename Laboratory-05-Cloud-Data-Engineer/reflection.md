# Reflection

## 1. Why is Object Storage better suited for the client’s photo-sharing application than Block Storage?

Object Storage is better suited because the application needs to store a large number of images. Object Storage is designed for unstructured data such as photos and can organize files as objects inside buckets. For a photo-sharing application, this makes it suitable for storing and accessing many uploaded images.

## 2. What was the most challenging part of deploying MinIO with Docker?

The most challenging part was deploying MinIO and making sure the container was running correctly. I needed to use the correct Docker command, environment variables, and port configuration. Checking the `docker ps` command helped me confirm that the MinIO container was running and that ports 9000 and 9001 were available.

## 3. In your own words, what is a “bucket” in Object Storage?

A bucket is a container used to organize and store objects. In this activity, I created a bucket named `client-photos` where the uploaded test image was stored. It is similar to a folder in a file system, but it is used to organize objects in Object Storage.

## 4. Why do enterprises care about Object Storage durability?

Enterprises care about durability because they store important amounts of data that need to remain available and protected. Object Storage is useful for large amounts of unstructured data, such as images and backups. Reliable storage helps organizations manage their data for long-term use.

## 5. How confident are you now with Linux command-line tools compared to before this lab?

I am more confident using Linux command-line tools after completing this activity. I was able to use Docker commands, check running containers, and deploy a storage service. I still need more practice, but this laboratory helped me become more comfortable with the Linux terminal.
