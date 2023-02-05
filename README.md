# Code for potential analysis

This repo includes the skeleton you will use to implement the potential analysis method. In the end, what we expected to be implemented?

* Image processing methodologies to extract and track a Silica microparticle in a .mp4 video.
* Potential analysis. With the coordinates for the center of mass of the particle extracted via image processing, a `curve_fit` is executed on the probability distribution of the coordinates. The fit results in the extraction of the trap stifness in the $x$ and $y$ directions.

## Installation

Well, now, how can you run this code? Follow the next steps.

1. First clone this repo in your computer. This can be done
    * Via SSH:

    ```bash
    git clone https://github.com/QuantumAdventures/cbpf-potential-analysis.git
    ```

    * Via HTTPS:

    ```bash
    git clone git@github.com:QuantumAdventures/cbpf-potential-analysis.git
    ```

    * Or, by downloading the .zip of the repo and unziping in your computer.

2. Install the requirements, this will set the libraries needed with the correct version in your computer. Inside the main folder of the project run the following command:

```bash
pip install -r requirements.txt
```

3. Create the data folder! You can do this navigating the file explorer of your computer. If you prefer, simply run the following command in the terminal:

    ```bash
    mkdir -p data/dataframes data/images data/videos
    ```
    
In the end you should have the following directory structure:


    ├── data
    │   ├── dataframes
    │   ├── images
    │   └── videos
    ├── notebooks
    │   ├── 1. Create frames from video.ipynb
    │   ├── 2. Microparticle detection and tracking.ipynb
    │   ├── 2.1. Execute detection for multiple images.ipynb
    │   ├── 3. Potential Analysis.ipynb
    ├── LICENSE
    ├── README.md
    └── requirements.txt


## License

This code is licensed by:

General Public License version 3.0 [GPL-3.0](https://choosealicense.com/licenses/gpl-3.0/)


Copyright (C) 2022  Quantum Adventures: Pontifical University of Rio de Janeiro
research group for optomechanics, quantum optics and quantum information.

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program.  If not, see <https://www.gnu.org/licenses/>.
