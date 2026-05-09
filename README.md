# Remote Desktop Connection via GitHub Actions and Tailscale By Ventra

This repository uses GitHub Actions to automatically create a remote desktop connection via Tailscale, allowing secure access to a Windows environment. Each GitHub Action execution generates an Tailscale tunnel that lasts for approximately 6 hour, enabling RDP (Remote Desktop Protocol) access.

### Key Features:
- **Automated Setup**: Uses GitHub Actions to set up and configure a remote desktop session.
- **Secure Tunnel**: Tailscale provides a secure tunnel for RDP access.
- **Quick Access**: Each session lasts about 1 hour, with easy reconnection using the IP provided by Tailscale.

### Installation & Setup:
1.Install tail scale then make an account.
2. Fork the repository.
3. Replace the TS_AUTH` in the GitHub Actions workflow file with your Tailscale authentication token.
4. Set the `TS_AUTH` in GitHub by adding it as an environment variable in your repository’s secrets.
5. Go to **Settings > Secrets > Actions** in your GitHub repo and add a new secret named `TS_AUTH`.
6. Go to **Actions > Cl > Run Workflow
7. Open Remote Desktop in ur pc ( Win + R > mstsc)
8. Put The ip u got from tailscale
9 The Default Credentials is : Username : runneradmin Password : P@ssw0rd!

### Warning:
1. U need to install tailscale in ur pc and make account in order for this to work
2.this is not for gaming dumbass this is for server and dont even try to play games btw this doesnt even have a graphics card
3.the workflow will end after 6 hour we cant do anything abt this so just rerun after 6 hour
4.The data will always reset after u rerun

### Contributing:
Feel free to submit pull requests or open issues for improvements or bug fixes.
