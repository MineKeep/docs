---
description: How to add Fabric mods to your MineKeep Server
icon: puzzle-piece
---

# Adding mods

{% hint style="danger" %}
MineKeep servers **only** support **Fabric** mods. Please ensure you do not attempt to install Forge or NeoForge mods, as they will not work.
{% endhint %}

Fabric mods are a way to change the gameplay or add new content to your server. Unlike plugins, mods generally require players to have the same mods installed on their client to connect.

**Important:** Most Fabric mods require the **Fabric API** mod to be installed as well. You should treat Fabric API as an essential installation before adding other mods.

## Method 1: Using the Mod Manager (Recommended)

The easiest and fastest way to install mods and modpacks is directly through our built-in Mod Manager on the panel. This automatically handles finding, downloading, placing, and removing the mod files for you.

### Accessing the Mod Manager

1. Go to the [MineKeep Dashboard](https://minekeep.net/servers) and select the cog icon next to the start button of your server to open the server management page.
2. In the navigation menu, click on the **Mods** tab. This will open the Mod Manager popup.

<figure><img src="../.gitbook/assets/mod-manager-navigation.png" alt="Navigating to the Mods tab"><figcaption></figcaption></figure>

### Browsing and Installing Mods

When you open the Mod Manager, you will see three main sections: **Browse**, **Installed**, and **Modpacks**. 

1. Ensure you are on the **Browse** section.
2. Use the **filter options** to choose which platform you want to search through: Modrinth or CurseForge.
3. Type the name of the mod into the **search bar** to find what you are looking for.
4. Once you have located the correct mod, click the button to install it directly to your server.

<figure><img src="../.gitbook/assets/mod-manager-browse.png" alt="The Browse tab in the Mod Manager"><figcaption></figcaption></figure>

### Installing Modpacks

If you want to install an entire pre-made collection of mods, you can use the **Modpacks** tab! 

This works exactly like the Browse tab, but instead of searching for individual mods, it searches through full modpacks hosted on Modrinth and CurseForge. Simply find the modpack you want and click install to apply it to your server.

<figure><img src="../.gitbook/assets/mod-manager-modpacks.png" alt="The Modpacks tab in the Mod Manager"><figcaption></figcaption></figure>

### Managing Installed Mods & Easy Client Downloads

If you want to view the mods you already have or remove one you no longer need, navigate to the **Installed** section. 

Here, you will see a list of all your currently installed mods, complete with their icon and version number. To remove a mod, simply click the **Uninstall** button next to it. 

**Downloading Mods for your Client:** Because players need the exact same mods installed on their computer to join your server, we've made this easy! You can click the **Download** button on the Installed page to automatically bundle all your server's mods into a `.zip` file and download them straight to your device. 

<figure><img src="../.gitbook/assets/mod-manager-installed.png" alt="The Installed tab in the Mod Manager"><figcaption></figcaption></figure>

*Note: After installing or uninstalling mods, you will need to restart your server to apply the changes!*

---

## Method 2: Manual Installation

If a specific mod isn't available on the Mod Manager, or if you are uploading a custom mod, you can still install it manually. 

### Step 1: Finding and downloading Fabric mods

Before you install a mod manually, you first need to find and download the `.jar` file. We recommend the use of either [CurseForge](https://www.curseforge.com/minecraft/search?class=mc-mods) or [Modrinth](https://modrinth.com/mods) for downloading mods. Below are guides on how to download the correct Fabric version from each platform:

{% tabs %}
{% tab title="CurseForge" %}
To download a mod from [CurseForge](https://www.curseforge.com/minecraft/search?class=mc-mods), you first need to find a mod you want to install.

**Searching for a specific mod**

You can search for a specific mod by using the search bar at the top of the CurseForge website.

<figure><img src="../.gitbook/assets/curseforge-mods-search.png" alt=""><figcaption></figcaption></figure>

Type the name of the mod you want, and press enter. Select the correct mod from the list of results.

**Downloading the Fabric version**

Once you are on the mod's page, do **not** click the main download button immediately. Instead, click on the **Files** tab. This is crucial to ensure you get the Fabric version and not the Forge version.

<figure><img src="../.gitbook/assets/curseforge-mods-files.png" alt=""><figcaption></figcaption></figure>

From the Files list, you must filter by your **Game Version** (e.g., 1.20.1) and ensure the **Mod Loader** is set to **Fabric**.

<figure><img src="../.gitbook/assets/curseforge-mods-platforms.png" alt=""><figcaption></figcaption></figure>

Once you find the file that matches your version and says "Fabric", click the three dots icon, and select the "Download file" button from the list of options.

<figure><img src="../.gitbook/assets/curseforge-mods-download.png" alt=""><figcaption></figcaption></figure>

You should now have a .jar file downloaded to your device. You can now continue on to the rest of the tutorial below.
{% endtab %}

{% tab title="Modrinth" %}
To download a mod from [Modrinth](https://modrinth.com/mods), you first need to find a mod you want to install.

**Searching for a specific mod**

You can search for a desired mod on Modrinth via the search bar found on the mods page.

<figure><img src="../.gitbook/assets/modrinth-mods-search.png" alt=""><figcaption></figcaption></figure>

From here, you can enter the name of the mod you wish to download. To make things easier, you can select "Fabric" under the "Loader" filter on the left side of the page.

**Downloading the Fabric version**

Now that you have selected the mod you want to download, you should be on the mod's resource page. Click the "Versions" tab or the green "Download" button.

<figure><img src="../.gitbook/assets/modrinth-mods-download.png" alt=""><figcaption></figcaption></figure>

**Crucial Step:** When looking at the list of versions, you must ensure the file is tagged with **Fabric**. Do not download files tagged only with "Forge" or "NeoForge".

<figure><img src="../.gitbook/assets/modrinth-mods-platforms.png" alt=""><figcaption></figcaption></figure>

After verifying the version is for Fabric, click the download button (usually a small download icon) to save the .jar file onto your device.

You can now continue on to the rest of the tutorial below.
{% endtab %}
{% endtabs %}

### Step 2: Uploading to your server

Now that you have the Fabric mod you want to add to your server, go to the [MineKeep Dashboard](https://minekeep.net/servers) and select the cog icon next to the name of your server. This will bring you to the management page for your server. It should look something like this:

<figure><img src="../.gitbook/assets/server-console.png" alt=""><figcaption></figcaption></figure>

From here, you can click on the button that says "Files". This will bring you to the file manager for your server. It should look something like this:

<figure><img src="../.gitbook/assets/server-mods-files.png" alt=""><figcaption></figcaption></figure>

If you do not see the **"mods"** folder, you can create one by clicking the Create a folder button highlighted below (ensure you name it `mods` in all lowercase):

<figure><img src="../.gitbook/assets/server-createfolder.png" alt=""><figcaption></figcaption></figure>

Now that you have a "mods" folder, select the folder by clicking it, and then click the upload button (the button to the right of the Create a folder button). This will bring up an upload dialog that allows you to either select a file, or drag a file on to it. From here, you can select the main area of the dialog, which will open a file selection window. Use this to navigate to the .jar file you previously downloaded, then select it. This will upload the mod to your MineKeep server.

---

## Important Notes on Fabric Mods

Regardless of whether you used the Mod Manager or installed them manually, keep these things in mind:

1. **Fabric API:** Almost all Fabric mods require a separate mod called [**Fabric API**](https://modrinth.com/mod/fabric-api) to work. Please ensure this is installed alongside your other mods.
2. **Dependencies:** Check the mod's download page for other requirements. Some mods require libraries like "Cloth Config" or "Architectury".
3. **Restart:** You must restart your server for mods to load.
4. **Client Installation:** Remember, if the mod adds new blocks or items, you must install the exact same mod version on your own Minecraft client to join the server.