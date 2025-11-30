# Tailscale Setup Guide

This guide explains how I connected my TrueNAS SCALE server to my Tailscale network (tailnet), allowing secure access to my server from outside my local network.

---

## What is Tailscale?

Tailscale is a simple mesh VPN that creates a secure private network between your devices using the WireGuard protocol. Your private Tailscale network is called a **tailnet**.

In practice, this allows your devices to communicate as if they were on the same local Wi-Fi network—without port forwarding or complex firewall configuration.

---

## Requirements

1. A TrueNAS SCALE server with admin access  
2. A computer outside your local network from which you want to access the server  
3. A Tailscale account (the free tier works) with admin access to your tailnet  

---

## Setup Steps

### 1. Generate an Auth Key

You’ll need an authentication key to connect your TrueNAS server to your tailnet.

1. Sign in to your Tailscale account.  
2. Go to **Settings → Keys** in the Tailscale admin console.  
3. Click **Generate auth key**.  
4. Enter a description (e.g., “TrueNAS SCALE Server”) and click **Generate Key**.  
5. Copy and save the key—you’ll use it in the next step.

---

### 2. Install and Configure Tailscale on TrueNAS

1. Open **TrueNAS SCALE** and go to the **Apps** tab.  
2. Select **Discover Apps**, then find and install the **Tailscale** app.  
3. After installation, click **Edit** on the Tailscale app.  
4. Paste your Auth Key into the **Auth Key** field.  
5. Set the **Hostname** field to whatever name you want your server to use on the tailnet.  
6. Under **Network Configuration**, select **Host Network** to bind the VPN to the host’s network.  
7. Click **Save**.

---

### 3. Verify the Connection

1. Open the Tailscale Admin Console.  
2. Go to the **Machines** page.  
3. Confirm that your TrueNAS SCALE server appears in your tailnet list. The adress under the **Addresses** tab is what you will use in place of your server's local network IP address in your browser's address bar to access your truenas management console. 

For the device that you want to use to access your server. Download the truenas application like any other vpn, then turn it on when you want to be connected to the tailnet. 

    

