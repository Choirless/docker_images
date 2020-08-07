# https://github.com/apache/openwhisk/blob/master/docs/actions-docker.md
FROM choirless/librosa_ml:release-2.4

RUN apt-get update && \
    apt-get install -y libsm6 libxext6 libxrender-dev git \
    && rm -rf /var/lib/apt/lists/*

RUN pip3 install importlib_resources \
    "choirless_smiler>=1.1.0" \
    aiohttp \
    "git+https://github.com/Choirless/renderer@b7ef5e2314018800159cb3a556cad0b2b7c142fe#egg=choirless_lib&subdirectory=python/choirless_lib"
    

