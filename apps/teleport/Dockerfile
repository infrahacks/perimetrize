FROM public.ecr.aws/gravitational/teleport:11.3.3

COPY ./teleport.yaml /etc/teleport/teleport.yaml
COPY ./bootstrap.yaml /etc/teleport/bootstrap.yaml

ENTRYPOINT [ "teleport", "start", "-c", "/etc/teleport/teleport.yaml", "--bootstrap", "/etc/teleport/bootstrap.yaml" ]
