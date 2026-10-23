# Third-party notices

Sorify © 2026 Anthony Fararoni is covered by its [EULA](LICENSE.md). The components below are either shipped with the installer or downloaded by it into Sorify's private runtime. Each one stays under its own license, reproduced or referenced here as those licenses require.

## OpenAI Whisper

Speech recognition: code and model weights. https://github.com/openai/whisper — MIT License

```text
Copyright (c) 2022 OpenAI

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

## PyTorch

Deep-learning runtime. https://pytorch.org — BSD-3-Clause License, Copyright (c) 2016- Facebook, Inc (Adam Paszke) and contributors; see https://github.com/pytorch/pytorch/blob/main/LICENSE. Builds with CUDA support include NVIDIA CUDA libraries under the [NVIDIA Software License Agreement](https://docs.nvidia.com/cuda/eula/).

## FFmpeg

Audio decoding (`ffmpeg.exe`, `ffprobe.exe`). https://ffmpeg.org — GNU Lesser General Public License v2.1 or later. Sorify downloads the `win64-lgpl-shared` build published by [BtbN/FFmpeg-Builds](https://github.com/BtbN/FFmpeg-Builds), which also provides the corresponding source code. Sorify runs FFmpeg as a separate program and does not link against it. License text: https://www.gnu.org/licenses/old-licenses/lgpl-2.1.html

## Python and Tcl/Tk

Private runtime. https://www.python.org — Python Software Foundation License, version 2, Copyright (c) 2001 Python Software Foundation; All Rights Reserved. The runtime is a build from [python-build-standalone](https://github.com/astral-sh/python-build-standalone) (MIT License, Copyright (c) 2019 Gregory Szorc). Full license texts ship in `runtime\LICENSE.txt`.

Tcl/Tk: https://www.tcl.tk — Tcl/Tk License (BSD-style), Regents of the University of California, Sun Microsystems, Scriptics, ActiveState and others.

## Python packages installed into the runtime

| Package | License | Copyright |
|---|---|---|
| [customtkinter](https://github.com/TomSchimansky/CustomTkinter) | MIT | (c) 2023 Tom Schimansky |
| [tkinterdnd2](https://github.com/Eliav2/tkinterdnd2) | MIT | (c) 2020 Philippe Gagne; bundles [TkDND](https://github.com/petasis/tkdnd), BSD-style, (c) Petasis Georgios |
| [NumPy](https://numpy.org) | BSD-3-Clause | (c) NumPy Developers |
| [Numba](https://numba.pydata.org) | BSD-2-Clause | (c) Anaconda, Inc. |
| [llvmlite](https://github.com/numba/llvmlite) | BSD-2-Clause | (c) Continuum Analytics, Inc. |
| [tiktoken](https://github.com/openai/tiktoken) | MIT | (c) 2022 OpenAI, Shantanu Jain |
| [tqdm](https://github.com/tqdm/tqdm) | MPL-2.0 and MIT | (c) noamraph and contributors |
| [more-itertools](https://github.com/more-itertools/more-itertools) | MIT | (c) 2012 Erik Rose |
| [darkdetect](https://github.com/albertosottile/darkdetect) | BSD-3-Clause | (c) 2019 Alberto Sottile |
| [regex](https://github.com/mrabarnett/mrab-regex) | Apache-2.0 | |
| [requests](https://github.com/psf/requests) | Apache-2.0 | |

plus their dependencies (certifi, charset-normalizer, idna, urllib3, colorama, filelock, fsspec, Jinja2, MarkupSafe, mpmath, networkx, sympy, typing_extensions, setuptools), each under its own permissive license recorded in the package's `dist-info` folder inside `runtime\Lib\site-packages`.

## Installer

Built with [Inno Setup](https://jrsoftware.org/isinfo.php), (c) Jordan Russell and Martijn Laan, used under the Inno Setup License.
