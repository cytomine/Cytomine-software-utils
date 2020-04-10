# Copyright (c) 2009-2020. Authors: see NOTICE file.
#
# Licensed under the Apache License, Version 2.0 (the "License");
# you may not use this file except in compliance with the License.
# You may obtain a copy of the License at
#
#      http://www.apache.org/licenses/LICENSE-2.0
#
# Unless required by applicable law or agreed to in writing, software
# distributed under the License is distributed on an "AS IS" BASIS,
# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
# See the License for the specific language governing permissions and
# limitations under the License.

FROM cytomine/software-java8-base:v2.0.0

RUN apt update -y && apt install -y zip unzip

RUN cd /tmp && \
    wget http://dl.bintray.com/groovy/maven/apache-groovy-binary-2.4.4.zip && \
    unzip apache-groovy-binary-2.4.4.zip && \
    mv groovy-2.4.4 /groovy && \
    rm apache-groovy-binary-2.4.4.zip

ENV GROOVY_HOME /groovy
ENV PATH $GROOVY_HOME/bin/:$PATH
