# FBR25-Electronics

## Setting up Footprint and Symbol libraries

1. Clone this repository to a sensible place on your PC, e.g. inside `Documents/FBR/`. Remember where it is stored.

2. Install the symbol library:

   1. In KiCad, click **Preferences** > **Manage Symbol Libraries**. Ensure you are on the **Global Libraries** tab in the dialog box.

   2. Click the open button in the bottom left. Navigate to where you cloned this repository and open `FBR-Symbols.kicad_sym`. Click OK.
  
3. Install the footprint library:

   1. In KiCad, click **Preferences** > **Manage Footprint Libraries**. Ensure you are on the **Global Libraries** tab in the dialog box.

   2. Click the open button in the bottom left. Navigate to where you cloned this repository and open `FBR-Footprints.pretty`. Click OK.
  
4. Setup the 3D symbol library: (This step is optional, but will make both the 3D view of your PCB, and any exported 3D models, much more complete)

   1. In KiCad, click **Preferences** > **Configure Paths...**.

   2. Click the "+" icon to add a new entry. Set "Name" to `FBR_3D_MODELS`.

   3. Set "Path" to the location of this repository, followed by `FBR_3D_MODELS` - for example, `/home/oliver/Documents/FBR/FBR25-Electronics/FBR_3D_MODELS`.

   4. Click OK.

## Creating a PCB Project

1. Create a new respository, using the template, by going to [the template repository](https://github.com/Full-Blue-Racing/ElectronicsProjectTemplate), and pressing "Use This Template"

2. Clone your repository to your local machine using `git clone https://github.com/Full-Blue-Racing/<project name>`.

3. Create the `generated` directory inside the repository. This should not be and doesn't need to be committed to GitHub.

4. Create a new KiCad project inside the repository, ensuring to uncheck "Create a new folder for the project".

## Submitting for Manufacturing

Once your project is complete, you can submit your PCB for review, and once we've checked it over it will be sent to be manufactured with the next batch of PCBs we order.

1. Create a release on GitHub.
   Ensure you've pushed all of your changes, then follow [Creating a Release](https://docs.github.com/en/repositories/releasing-projects-on-github/managing-releases-in-a-repository#creating-a-release).
   You should also export the Gerbers for your PCB, and a Bill of Materials, and upload these to the release page.

2. Submit your release [here](https://forms.gle/mBnbXawvQiZjMk937).

3. Once reviewed, we will also add your PCB into the main Loom schematic.
