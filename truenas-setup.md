# TrueNAS Setup Guide

> **NOTE:** The procedure described below will **wipe all involved
> drives** during installation. Proceed with caution.

## Requirements

-   **USB boot drive** (Ventoy recommended, but any tool works)
-   **Computer/Server** to install TrueNAS SCALE on
    -   Must have **at least two drives**:
        -   One internal boot drive
        -   One secondary drive for storage
-   **Stable internet connection** and **router with admin access**

## Initial Setup

1.  Download TrueNAS:

    -   Navigate to:\
        **https://www.truenas.com/download-truenas-community-edition/**\
        Download the latest version of **TrueNAS SCALE** (may now appear
        as *TrueNAS Community Edition*).

2.  Create a bootable USB drive:

    -   Download the `.iso` and copy it to your USB boot drive.

3.  Install TrueNAS:

    -   Power down the target system.
    -   Insert the USB boot drive.
    -   Boot from USB and follow installation prompts.
    -   Install the OS on your **internal boot drive**.

4.  After installation, you should see the console setup menu.
![alt text](ConsoleSetupMenuSCALE.png)

5.  From another device on the same network, open the URL displayed on
    the TrueNAS console screen.

6.  Create your web UI **username and password**.

## Dataset Creation

A **dataset** is a filesystem-like container within a **storage pool**.
Think of it as a folder with additional features such as quotas and
snapshots.

### Create a Storage Pool

1.  Go to **Storage** in the left sidebar.
![alt text](image.png)
2.  Click **Create Pool**.
![alt text](image-1.png)
3.  Name your pool (e.g., `Main`).
4.  Select a layout:
    -   With **one drive**, choose **Stripe** (no redundancy).
    -   For redundancy, choose **Mirror** (requires two drives).
5.  Review and click **Create Pool**.

### Create a Dataset

Once the pool exists, you can create datasets inside it.

(More instructions coming soon.)
