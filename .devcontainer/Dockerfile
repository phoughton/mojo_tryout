FROM phoughton/python-dev-main


USER vscode

RUN curl https://get.modular.com | sh - && \
modular auth mut_da80461f59854ff9ac3e075713229950

RUN modular install mojo

RUN echo "export MODULAR_HOME=\"/home/vscode/.modular\"" >>  ~vscode/.bashrc && \
    echo "export PATH=\"/home/vscode/.modular/pkg/packages.modular.com_mojo/bin:$PATH\"" >> ~vscode/.bashrc 
    