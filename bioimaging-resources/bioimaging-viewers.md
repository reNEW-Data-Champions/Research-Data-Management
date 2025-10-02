---
description: Open-Source Bioimage Viewers
layout:
  width: wide
  title:
    visible: true
  description:
    visible: true
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
  metadata:
    visible: true
---

# 🟤 Bioimaging Viewers

#### Here is a list of Open-source viewers best suited for life-science microscopy (fluorescence/confocal/spinning-disk, widefield, light-sheet, live-cell, EM/WSI).

<table data-header-hidden><thead><tr><th width="162" valign="top"></th><th width="183" valign="top"></th><th width="200" valign="top"></th><th width="165" valign="top"></th><th width="166" valign="top"></th><th valign="top"></th></tr></thead><tbody><tr><td valign="top">Name</td><td valign="top">Platform (OS)</td><td valign="top">Primary modalities</td><td valign="top">N-D support (C/Z/T)</td><td valign="top">File format backbone</td><td valign="top">Notable limitations / caveats</td></tr><tr><td valign="top">Fiji (ImageJ)</td><td valign="top">Desktop (Win/macOS/Linux)</td><td valign="top">Widefield, confocal, light-sheet, EM; everything from single fields to mosaics</td><td valign="top">2D–5D (C/Z/T)</td><td valign="top">Bio-Formats, OME-TIFF</td><td valign="top">Performance on very large datasets needs care (RAM, tiling); UI can feel legacy; plugin quality varies</td></tr><tr><td valign="top">napari</td><td valign="top">Desktop (Win/macOS/Linux; Python)</td><td valign="top">Fluorescence/confocal/light-sheet; interactive labeling/annotation; N-D arrays</td><td valign="top">2D–5D</td><td valign="top">Readers for OME-TIFF, Zarr, and many plugins</td><td valign="top">Ecosystem still maturing in some niches; requires Python setup for best use</td></tr><tr><td valign="top">Icy</td><td valign="top">Desktop (Win/macOS/Linux)</td><td valign="top">Fluorescence/confocal/time-lapse; interactive workflows</td><td valign="top">2D–4D</td><td valign="top">Bio-Formats, TIFF/OME-TIFF</td><td valign="top">Smaller ecosystem vs Fiji/napari; fewer cutting-edge big-data tools</td></tr><tr><td valign="top">QuPath</td><td valign="top">Desktop (Win/macOS/Linux)</td><td valign="top">Brightfield/IF pathology, WSI; tiles &#x26; tissue slides</td><td valign="top">2D (multi-channel)</td><td valign="top">Bio-Formats; pyramidal WSI formats; OME-TIFF</td><td valign="top">Primarily 2D WSI (less for Z/T stacks); microscopy timelapse/volumetric less central</td></tr><tr><td valign="top">OMERO.iviewer</td><td valign="top">Web (server-backed: OMERO)</td><td valign="top">Lab microscopy across modalities; central data portal</td><td valign="top">2D–5D</td><td valign="top">OME stack via OMERO</td><td valign="top">Requires OMERO server; analysis is limited vs desktop tools</td></tr><tr><td valign="top">BigDataViewer (Fiji plugin)</td><td valign="top">Desktop (Java; via Fiji)</td><td valign="top">Light-sheet, large 3D volumes, multi-view</td><td valign="top">3D/4D/5D</td><td valign="top">HDF5/N5; OME-TIFF via bridges</td><td valign="top">Viewer/IO focused; relies on Fiji for processing; learning curve</td></tr><tr><td valign="top">MoBIE (Fiji-based)</td><td valign="top">Desktop (Fiji plugin)</td><td valign="top">Cell/EM/light-sheet atlases; multi-modal big data</td><td valign="top">3D/4D/5D</td><td valign="top">N5/Zarr, OME-TIFF</td><td valign="top">Project structure conventions; best when adopting N5/Zarr</td></tr><tr><td valign="top">ilastik</td><td valign="top">Desktop (Win/macOS/Linux)</td><td valign="top">Fluorescence/confocal; interactive pixel/object classification, tracking</td><td valign="top">2D–4D</td><td valign="top">Bio-Formats, TIFF/OME-TIFF</td><td valign="top">More analysis than general viewer; limited general visualization features</td></tr><tr><td valign="top">BioImage Suite Web</td><td valign="top">Web (client-side)</td><td valign="top">General bioimage viewing/processing in browser</td><td valign="top">2D/3D</td><td valign="top">Standard image stacks (TIFF/NIfTI etc.)</td><td valign="top">Not optimized for huge microscope pyramids; fewer pro tools</td></tr><tr><td valign="top">3D Slicer</td><td valign="top">Desktop (Win/macOS/Linux)</td><td valign="top">Large volumetric imaging (lightsheet/OPT/μCT), registration/segmentation</td><td valign="top">3D/4D</td><td valign="top">NRRD, NIfTI, TIFF; plugins for OME-TIFF</td><td valign="top">Steeper learning curve for microscopy newcomers; medical defaults</td></tr></tbody></table>

#### Selection tips (quick guidance) <a href="#b0d42hrxqd92" id="b0d42hrxqd92"></a>

●     General lab viewer + broad analysis & scripting: Fiji (with Bio-Formats).\
●     Modern N-D visualization, Zarr, interactive labeling: napari.\
●     Whole-slide/tissue (brightfield & IF): QuPath.\
●     Very large 3D light-sheet / multi-view: BigDataViewer or MoBIE (N5/Zarr).\
●     Centralized, permissioned web viewing across a group/institute: OMERO.iviewer (with OMERO )

Note: Most desktop tools listed can open proprietary microscope formats (e.g., CZI, LIF, ND2) through Bio-Formats and work natively with OME-TIFF/OME-Zarr; for massive datasets, prefer pyramidal OME-TIFF or OME-Zarr (chunked, multi-resolution) for smooth viewing
