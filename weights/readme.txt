// split vgg16_weights_v1 into  10MB tar.gz files
tar -czvf - /share/vgg16_weights_v1.7z | split -b 10M - vgg16.tar.gz

//  uncompressed with:
cat vgg16.tar.* | tar -xzvf -
7z x share/vgg16_weights_v1.7z

