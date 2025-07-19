# Remote-SSH-For-Windows-Cloudflared-Tunnel
Remote SSH For Windows Cloudflared Tunnel


Download and install cloudflare :
winget install --id Cloudflare.cloudflared

Alternatively, download the latest release directly:
- 32Bit
https://github.com/cloudflare/cloudflared/releases/latest/download/cloudflared-windows-386.exe

- 64Bit
https://github.com/cloudflare/cloudflared/releases/latest/download/cloudflared-windows-amd64.exe



# Putty 
Download and install putty

putty - connection - proxy 
proxy hostname : ssh.example.com

command to send to proxy 
cloudflared.exe access ssh --hostname %host --> putty


# WinSCP
Download and install WinSCP

Advanced Site Settings
Connection - Proxy :
Proxy Type - local

local proxy command :
C:\Program Files (x86)\cloudflared\cloudflared.exe access ssh --hostname %host --> WinSCP
