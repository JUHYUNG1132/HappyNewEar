## 2021 19th KESSIA Embeded Software Contest Repo.
## Team HappyNewEar
이현제, 이주형, 이지수, 장예진, 정하연  

## Objective
System for Hard of Hearing  

## Result
**KESSIA Chairman's Awarded**  

## Project Overview
The system helps hearing-impaired people accurately and quickly recognize dangerous situations they may encounter in their daily lives (such as car horns, sirens, and gas explosions).  
It receives sounds through an omnidirectional microphone array, classifies them, and transmits the direction of the sound to a display and bone conduction speaker (via vibration).  

## Key Features
- Real-time Audio Classification: With YAMNet using TensorFlow Lite, classifies 47 sounds in real-time.   
- Sound Source Localization (SSL): Localize direction of incoming sound via 4-Mic-Array and ODAS
- Display: Visualize the position and type of sound using
- Bone conduction speaker: Vibrate to alert user in 3 levels of danger.
- On-device & Portable: Portable system using Raspberry-pi and power bank while all pipelines are processed on-device.

## Software
- Raspberry Pi OS (Linux)
- Python 3.7.3
- ML Framework: TensorFlow Lite

## Demo
Youtube Demo ==> [ytlink]  

[ytlink]: https://www.youtube.com/watch?v=RFun6zqWqaE "Demo link"  

## Repo Structure
├── Docs/                   # Project documentation (Proposals, Final report)  
├── deprecated/             # Unused or legacy files  
├── img/                    # Predicted class assets
├── odas/                   # External: ODAS repository (Vendored)
│  
├── HappyNewEar.sh          # Project executable shell script  
├── main_plt.py             # Main entry point (using Matplotlib for plotting)  
├── main_pygame.py          # Main entry point (using Pygame for plotting)  
├── Classification.py       # Audio classification core module  
│  
├── yamnet.tflite           # YAMNet model weights  
├── yamnet_class_map_*.csv  # Class label mapping for YAMNet predictions  
├── odas.cfg                # ODAS Configuration files  
│  
├── log.txt                 # Runtime logs  
└── README.md  
  
ODAS repo. ==> [odasLink]  

[odasLink]: https://github.com/introlab/odas "ODAS Repo."