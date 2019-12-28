## Buildstage ##
FROM lsiobase/alpine:3.9 as buildstage

# copy local files
COPY root/ /root-layer/

## Single layer deployed image ##
FROM scratch

# Add files from buildstage
COPY --from=buildstage /root-layer/ /
