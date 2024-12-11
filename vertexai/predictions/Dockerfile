FROM asia-docker.pkg.dev/vertex-ai/prediction/pytorch-gpu.2-1:latest
ENV AIP_HEALTH_ROUTE /ping
ENV AIP_PREDICT_ROUTE /predictions/model

RUN pip install transformers

USER root
RUN chown -R model-server:model-server /home/model-server

USER model-server
ENTRYPOINT ["python", "entrypoint.py"]

