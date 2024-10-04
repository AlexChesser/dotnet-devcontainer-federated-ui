FROM mcr.microsoft.com/devcontainers/dotnet:1-8.0-jammy

# Install VS Code Server
RUN mkdir -p /root/.vscode-server/extensions
RUN curl -fsSL https://update.code.visualstudio.com/latest/server-linux-x64/stable | tar -C /root/.vscode-server -xzf -

# Install VS Code extensions
RUN /root/.vscode-server/bin/*/bin/code-server --install-extension ms-dotnettools.vscode-dotnet-runtime \
    && /root/.vscode-server/bin/*/bin/code-server --install-extension ms-dotnettools.csharp \
    && /root/.vscode-server/bin/*/bin/code-server --install-extension dbaeumer.vscode-eslint \
    && /root/.vscode-server/bin/*/bin/code-server --install-extension GitHub.copilot \
    && /root/.vscode-server/bin/*/bin/code-server --install-extension GitHub.copilot-chat