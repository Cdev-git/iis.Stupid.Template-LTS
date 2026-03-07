# ii's Stupid Template-LTS
ii's Stupid Template LTS is a mod menu template for Gorilla Tag with custom categories and the maximum amount of customization possible. This template is meant for more advanced users, so if you're a new menu creator, this could be difficult for you.

## Do I need permission to use this?
No, this template is free and public for anyone to use. You are welcome to utilize it for your projects, modify it to suit your needs, and share it with others. We believe in a collaborative and open community where resources are accessible to all.

---

# Installation
- Go to https://github.com/Cdev-git/iis.Stupid.Template-LTS/releases/tag/v1.0.0 and download the zip file
- Change your `<GamePath>` (Gorilla Tag directory) in `Directory.Build.props` if required
- Change the menu name in `PluginInfo.cs`
- Edit the menu visuals in `Menu/Settings.cs`
- Add buttons in `Menu/Buttons.cs`
- Build with `Ctrl` + `Shift` + `B`, it will get put in your plugins folder automatically


# Mod example
## Teleport to stump
public static void TP_Stump()
{
    GTPlayer.Instance.TeleportTo(new Vector3(-68.647f, 12.406f, -83.699f), GTPlayer.Instance.transform.rotation, false, true);
    GorillaTagger.Instance.rigidbody.linearVelocity = Vector3.zero;
}
