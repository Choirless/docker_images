# https://github.com/apache/openwhisk/blob/master/docs/actions-docker.md
FROM choirless/librosa_ml:release-2.6

RUN apt-get update && \
    apt-get install -y libsm6 libxext6 libxrender-dev git \
    && rm -rf /var/lib/apt/lists/*

RUN pip3 install importlib_resources \
    "choirless_smiler>=1.2.1" \
    matplotlib \
    pykalman \
    aiohttp \
    "git+https://github.com/Choirless/renderer@e0f2c46d5e4b2a34fa67b034f141fb286cffab2a#egg=choirless_lib&subdirectory=python/choirless_lib"


    

