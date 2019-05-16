# Go cross compiler (xgo): Go 1.11.x
# Copyright (c) 2018 Péter Szilágyi. All rights reserved.
#
# Released under the MIT license.

FROM karalabe/xgo-latest


RUN apt-get update && apt-get install -y cmake 

# Add patches directory for patching later
ADD patches /patches

COPY iPhoneSimulator9.3.sdk.tar.gz /iPhoneSimulator9.3.sdk.tar.gz
RUN ls /iPhoneSimulator9.3.sdk.tar.gz
RUN /update_ios.sh iPhoneSimulator9.3.sdk.tar.gz

MAINTAINER Péter Szilágyi <peterke@gmail.com>
