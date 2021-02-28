FROM fedora:33
RUN set -ex; yum clean all && \
    yum install -y python3-scipy python3-numpy python3-pandas python3-networkx python3-matplotlib python3-scikit-learn python3-requests python3-argon2-cffi python3-wheel python3-pip && \
    pip install jupyterlab && yum clean all && mkdir /jupyter
WORKDIR /jupyter
CMD ["jupyter-lab", "--allow-root", "--no-browser", "--ip=0.0.0.0"]
