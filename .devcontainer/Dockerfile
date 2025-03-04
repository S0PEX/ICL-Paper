# Use the latest full version of TeX Live as the base image
FROM texlive/texlive:latest-full

# Update the package list and install necessary packages
# It's a good practice to clean up after installing packages to reduce image size
RUN apt update && apt install -y \
    tex-fmt \
    && apt clean \
    && rm -rf /var/lib/apt/lists/*

# Install tex-fmt (alternative to latexindent)
RUN apt install tex-fmt