FROM mxnet/python:latest_cpu_native_py3

ADD examples/v1beta1/trial-images/mxnet-mnist /opt/mxnet-mnist
WORKDIR /opt/mxnet-mnist

RUN chgrp -R 0 /opt/mxnet-mnist \
  && chmod -R g+rwX /opt/mxnet-mnist

ENTRYPOINT ["python3", "/opt/mxnet-mnist/mnist.py"]
