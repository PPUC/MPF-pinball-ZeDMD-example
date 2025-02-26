# MPF pinball ZeDMD demo

## Running steps

- Install Godot
- Create and activate a python environnement
- Run this commands :
```shell
pip install numpy

git clone https://github.com/PPUC/mpf-zedmd.git
cd mpf-zedmd
git checkout 0.80.x
pip install -e .

cd ..
git clone https://github.com/PPUC/MPF-pinball-ZeDMD-example.git

cd MPF-pinball-ZeDMD-example

mpf

```
- Run Godot
  - Open project.godot
  - Run the project


## How does it works ?
Look at Anthony van Winkle post here : https://groups.google.com/g/mpf-users/c/eTe_1PEFQq4/m/Kl4Vp8FdBAAJ

> You can see in the config.yaml the hardware configuration I setup, yours will of course vary but there is no requirement for window: or displays: sections. There is one important thing you need to configure and that's the name of the dmd (under the rgb_dmds: section). In the sample repo it's named fast_rgb_dmd, and in the godot scene dmd_window.tscn the main Window has a child node (of type MPFDMDDisplay) and the node name is also fast_rgb_dmd. It's necessary for you to make sure your DMD node name matches the rgb_dmd name in your config, because that's how MPF knows which DMD to update. 
