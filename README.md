# Setup
**Make sure to read the instructions carefully!**

If you have other resources used in the Blender project and chose to *make all paths relative*, pack all of them into a zip archive. Alternatively, you can *pack all external file*.

* `blender_version` : Unable to change version beacause linux eevee render support only blender 3.4.
* `blend_file_path` : Path to the blend file after unpacking the zip archive. If blend file is used, this is automatically ignored.
___
* `upload_type` : Select the type of upload method. `gdrive_relative` pulls everything from the folder specified.
* `drive_path` : Path to your blend/zip file relative to the root of your Google Drive if `google_drive` is selected. Must  state the file and its extension (.zip/.blend) **unless** `gdrive_relative` is selected.
* `url_blend` : Specify the URL to the blend/zip file if `url` is selected.
___
* `animation` : Specify whether animation or still image is rendered. If **still image** is used, put the frame number in `start_frame`.
* `start_frame, end_frame` : Specify the start and end frame for animation. You may put same value such as zero for both input to set the default frame in the blend file.
___
* `download_type` : Select the type of download method. `gdrive_direct` enables the frames to be outputted directly to Google Drive (zipping will be disabled).
* `output_name` : Name of the output frames, **do NOT include .blend!** (## for frame number)
* `zip_files` : Archive multiple animation frames automatically into a zip file.
* `drive_output_path` : Path to your frames/zip file in Google Drive.
___
* `gpu_enabled, cpu_enabled` : Toggle GPU and CPU for rendering. CPU might give a slight boost in rendering time but may varies depend on the project.
* `optix_enable` : Enable OptiX which may boost performance, may be incompatible depending on the version of blender, project and GPU allocated

After you are done, go to Runtime > Run All (Ctrl + F9) and upload your files or have Google Drive authorised below. See the [GitHub repo](https://github.com/filispeen/blender-render-eevee-and-cycles) for more information.
