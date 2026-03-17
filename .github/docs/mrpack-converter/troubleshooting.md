# 🛑 Troubleshooting the MRPACK Converter

Running into a wall while trying to convert your modpack? Don't worry! Most issues with the AméthMC MRPACK Converter are quick fixes related to browser limits or network connections.

Find your issue below to get back on track.

---

## 1. The progress bar is stuck at 99%
This is the most common issue for massive modpacks (250+ mods). 
* **The Cause:** The converter has downloaded all the mods, but your browser is struggling to zip them all together into a single file because it ran out of memory.
* **The Fix:** Try closing other heavy tabs or applications to free up RAM. If it consistently fails, try using a Chromium-based browser (Chrome, Edge, Brave) which generally handles large client-side memory tasks better than Safari or older browsers.

## 2. "Invalid File Type" or "File Not Recognized"
* **The Cause:** You might be trying to upload a standard `.zip` file, or the Modrinth `.mrpack` file you downloaded was corrupted during the download.
* **The Fix:** Make sure the file extension explicitly says `.mrpack`. If it does and it still fails, delete the file, go back to Modrinth, and download a fresh copy of the modpack.

## 3. Network Error / "Failed to Fetch"
* **The Cause:** The converter communicates directly with the Modrinth API to download your mods. Sometimes, Modrinth's servers get overloaded, or a strict ad-blocker/firewall on your network blocks the connection.
* **The Fix:** 1. Temporarily disable any aggressive ad-blockers or privacy extensions (like Privacy Badger or strict Brave Shields) for `amethmc.frisly.me`.
  2. Check [Modrinth's Status Page](https://status.modrinth.com/) to ensure their API isn't down.
  3. Wait 5 minutes and try again.

## 4. Some mods are missing after conversion!
* **The Cause:** `.mrpack` files don't actually contain the mods; they contain a list of links. Very rarely, a mod author deletes their mod from Modrinth, meaning the link in the `.mrpack` is dead. The converter will skip it rather than crashing the whole process.
* **The Fix:** The converter will usually warn you if it skips a file. You will need to manually find a replacement for that specific missing mod on Modrinth or CurseForge.

---

## 🆘 Still stuck?

If you've tried the steps above and the converter is still failing, we are here to help!

1. **[Join our Discord](YOUR_DISCORD_LINK)**: Hop into the support channel and ask the community or DevFrisly directly.
2. **[Report a Bug](https://github.com/DevFrisly/AmethMC-Utils/issues)**: If you believe the converter is genuinely broken, please open an issue and include the exact name and version of the modpack you are trying to convert.