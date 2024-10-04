FROM mcr.microsoft.com/devcontainers/dotnet:1-8.0-jammy

# install VS Code (code-server)
RUN curl -fsSL https://code-server.dev/install.sh | sh

# Install VS Code extensions
RUN code-server --install-extension ms-dotnettools.vscode-dotnet-runtime