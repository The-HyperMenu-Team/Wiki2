## 🪟 Windows

1. Download the latest **HyperMenu zip pack** from [here](https://github.com/ADHyperActive/MalumMenu/releases/latest).
    - **For Steam or Itch.io:** Download `HyperMenu-VERSION-Steam-Itch.zip`.
    - **For Microsoft Store, Epic Games Store, or Xbox App:** Not supported by HyperMenu. For these platforms, go to the original MalumMenu [here](https://github.com/scp222thj/MalumMenu/releases/latest).

2. Open the zip file you have just downloaded and copy all its contents.

3. Paste these files directly into your Among Us game folder:
    - **Steam:** Right-click Among Us in your Library → Click `Manage` → Click `Browse local files`.
    - **Itch.io:** Open the Itch.io app → Right-click Among Us in your Library → Click `Manage` → Click `Open folder in Explorer`.
    - **Epic Launcher:** Not currently supported by HyperMenu.
    - **Microsoft Store:** Not currently supported by HyperMenu.
    - **Xbox App:** Not currently supported by HyperMenu.

4. Launch Among Us as you normally would. You should see a console window appear, installing the mod's requirements.

5. Wait for the console window to finish the installation.

6. After installation, Among Us will automatically open with HyperMenu successfully installed.
    - By default, you can toggle the cheat GUI on by pressing **DELETE** on your keyboard.

7. If the installation doesn't work, check out our [FAQ](#-faq).

## 🐧 Linux

1. Run Among Us under **Proton (or Wine)**.
   - **In Steam:** Right-click Among Us in your Library → Click `Properties` → Click `Compatibility` → Enable `Force the use of a specific Steam Play compatibility tool`.

   - Test different Proton versions if you're having issues launching the game.

2. Set up **BepInEx** (the framework HyperMenu is built upon).
   - Follow the official Proton / Wine setup guide found [here](https://docs.bepinex.dev/articles/advanced/proton_wine.html).
   - If you are using Proton with Steam, specify the DLL override:
     - **In Steam:** Right-click Among Us in your Library → Click `Properties` → Click `General` → Click `Launch Options`.
     - Add this to your launch options:

       ```
       WINEDLLOVERRIDES="winhttp.dll=n,b" %command%
       ```

   - After that, continue with the Windows installation steps found [here](#-windows).

3. Fix crashes or errors (like `Unable to execute IL2CPP chainloader`).
   - **In Steam:** Right-click Among Us in your Library → Click `Properties` → Click `General` → Click `Launch Options`.
   - Set your launch options to:

     ```
     PROTON_NO_ESYNC=1 PROTON_USE_WINED3D=1 WINEDLLOVERRIDES="winhttp.dll=n,b" %command%
     ```