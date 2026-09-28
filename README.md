# Always Chant Crash Fix (FFT: TIC)

Fixes the `[fftivc.misc.alwayschant] AoB not found` startup crash.

### Option 1: Use the Patched File (Fastest)
Download `fftivc.misc.alwayschant.dll` and replace the one in your `Reloaded-II/Mods/fftivc.misc.alwayschant/` folder.

### Option 2: Patch It Yourself
1. Open `fftivc.misc.alwayschant.dll` in **dnSpy**.
2. Go to `Mod` > `Mod(ModContext)` > Right-click > **Edit IL Instructions...**
3. At line `49` (`ldstr`), replace the text with: `3C 03 0F 96 C1 45 85 FF 0F 85 BB 00 00 00 41 80 7D 00 5A`
4. Click **OK**, then **File** > **Save Module...** to overwrite the DLL.
