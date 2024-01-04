# Quick Summary for Importing Custom Music to Need for Speed Rivals

Tl;dr:

1. Have (or make) an MP3 file.

2. Convert the MP3 file to EALAYER3 using **bf2-sound-import's** **dandev-el3.exe** and note down the results for **ChunkSize** and **SegmentLength**.

3. In Frosty Editor, duplicate a **SoundWaveAsset** file and import the EALAYER3 file.
   * Check that **ChunkSize** value matches the output for **dandev-el3.exe**.
   * Set the value for **Selection** to **SoundWaveVariationSelection_Random**.
   * If the **SamplesOffset** value is **anything other than 0**, edit the value and set it to 0.
   * If the **SeekTableOffset** has a value of **0**, edit the value and set it to the following value: **4294967295**
   * Edit the **SegmentLength** value with the SegmentLength value from the **dandev-el3.exe** results.

4. Duplicate a **MusicAsset** file.
   * Edit the **NameHash** value to a unique 10-digit number.
   * Edit the **Title** and **Artist** vales accordingly.
   * Under the **Playables > [0]** property, paste the name of your MusicAsset in **Id** and **Name**.
   * On **Wave**, assign your **SoundWaveAsset**.
   * Under **Selectors > [0] > Target**, paste the name of your MusicAsset in **Id** and **Name**.

5. Open the **FreedrivePlaylist** file and under **Assets**, either:
   * Delete the original playlist and add a new item to **Assets**, and assign the (null) item with your **MusicAsset**, 
   
   * OR
   
   * Overwrite any existing item under **Assets** with your **MusicAsset**

6. **Export to Mod** and add the mod in Frosty Mod Manager.

7. Apply the mod and launch the game!
