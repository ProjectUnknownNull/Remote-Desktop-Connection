# Remote Desktop Connection via GitHub Actions

This repository uses GitHub Actions to automatically create a remote desktop connection via Tailsclae, allowing secure access to a Windows environment. Each GitHub Action execution generates an Tailsclae tunnel that lasts for approximately 1 hour, enabling RDP (Remote Desktop Protocol) access.

### Key Features:
- **Automated Setup**: Uses GitHub Actions to set up and configure a remote desktop session.
- **Secure Tunnel**: Tailscale provides a secure tunnel for RDP access.
- **Quick Access**: Each session lasts about 1 hour, with easy reconnection using the IP provided by Ngrok.

### Installation & Setup:
1. Fork the repository.
2. Replace the TS_AUTH` in the GitHub Actions workflow file with your Ngrok authentication token.
3. Set the `TS_AUTH` in GitHub by adding it as an environment variable in your repository’s secrets.
   - Go to **Settings > Secrets > Actions** in your GitHub repo and add a new secret named `NGROK_AUTH_TOKEN`.
4. Trigger the GitHub Action by pushing any change or using the **workflow_dispatch** event.
5. Once the action runs successfully, Ngrok will provide an IP address and port.
6. Use Remote Desktop Connection to connect to the provided IP and port.

### Contributing:
Feel free to submit pull requests or open issues for improvements or bug fixes.
