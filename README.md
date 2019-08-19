# SeetaFace2-Performance-Test
This repo is used to test seetface2 face recognition project performance

## Test process
1. Test with 640 * 480 and 1920 * 1080 image, consider the easiest case only one face in image;  
2. For detection and landmark run 1000 times, for extraction run 100 times;
3. Not count time spent on opencv draw point or bounding box.
## Hardware
i5-8400 CPU@ 2.80GHz
## performance
input size | 640 * 480 | 1920 * 1080
--------- | ------------- | -------------  
face detect(minsize 40) | 9.8ms | 55.8ms
face landmark(81 points) | 1.4ms | 1.6ms
face extract(resnet50) | 115.8ms | 116.3ms
