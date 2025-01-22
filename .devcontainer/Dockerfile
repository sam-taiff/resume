FROM ghcr.io/josiahbull/dotfiles:latest

# Install everything reuqired to build the resume.
RUN sudo apt-get update && sudo apt-get install -y texlive \
    texlive-fonts-recommended \
    texlive-fonts-extra \
    poppler-utils \
    texlive-xetex

# Install python + python packages that I use for normal development
RUN apt-get install -y python3 python3-pip
RUN pip3 install --break-system-packages thefuck pre-commit

# Set the shell to zsh
RUN chsh -s /bin/zsh
SHELL ["/bin/zsh", "-c"]
