FROM alpine:edge

ENV WEASYPRINT_VERSION=44

# ttf-dejavu is not used, but necessary to force Alpine into configuring fontconfig.
RUN apk add --no-cache gcc musl-dev jpeg-dev zlib-dev libffi-dev cairo-dev pango-dev gdk-pixbuf python3-dev fontconfig ttf-dejavu ca-certificates

RUN pip3 install weasyprint==$WEASYPRINT_VERSION

CMD [ "weasyprint", "--version" ]
