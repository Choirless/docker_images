# https://github.com/apache/openwhisk/blob/master/docs/actions-docker.md
FROM choirless/librosa_ml:release-2.4

RUN apt-get update && \
    apt-get install -y libsm6 libxext6 libxrender-dev git \
    && rm -rf /var/lib/apt/lists/*

RUN pip3 install importlib_resources \
    "choirless_smiler>=1.2.1" \
    aiohttp \
    "git+https://github.com/Choirless/renderer@8013eacede395f88b681cb9f7d108621c034a644#egg=choirless_lib&subdirectory=python/choirless_lib"


    

