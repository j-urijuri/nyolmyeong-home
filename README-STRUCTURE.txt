NYOL v171 structure

index.html
  - main homepage
  - HOME hosts MyHome through iframe
  - STUDIO > HOME is creator/admin status only

myhome/index.html
  - independent MyHome runtime
  - PLAY mode: character movement / future interactions
  - EDIT mode: furniture select, drag, nudge, rotate, save/cancel
  - same Three.js scene is shared by PLAY and EDIT
  - layout currently saved per AU in localStorage

myhome/assets/3d/
  - character01.glb
  - furniture/*.fbx

Next planned 3D step:
  Blender rig -> idle / walk / sleep clips -> export one GLB.
  Face expressions are planned as texture swaps on a FACE material.


v172 outdoor world
- myhome/index.html = OUTDOOR WORLD
- myhome/home.html = HOME INTERIOR
- house click: outdoor -> interior
- OUTSIDE button: interior -> outdoor
- no on-screen direction pad
- floor click/tap moves character
- house / bench clicks use interaction targets
- MAP button opens a lightweight minimap
- outdoor EDIT: drag/rotate/save selected decor
- uploaded outdoor FBX assets live under myhome/assets/3d/outdoor/
- current cottage is a temporary primitive HOUSE SLOT; replace it with a real house asset later.


v173 real outdoor asset pass
- uploaded house.fbx replaces the temporary primitive cottage
- separate left/right double-gate models are used
- tree + tree_large added around the outdoor map
- mailbox + letter + package added near the home path
- mailbox has a PLAY interaction target
- house click still moves to the door then loads home.html
