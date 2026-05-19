# tharu-humanoid-2026

Building [Asimov v1](https://github.com/asimovinc/asimov-1), an open-source bipedal humanoid robot, over summer 2026 in the UK. Full public build log: CAD modifications, firmware, training data, weekly write-ups.

**Status:** Kit deposit placed (May 2026). Hardware arrives August. Build runs June through September.

---

## About this project

I'm Tharu, a second-year BEng Electrical and Electronic Engineering undergraduate at Swansea University. I didn't get a summer internship this year, so I'm spending the summer building [Asimov v1](https://github.com/asimovinc/asimov-1), the open-source humanoid robot Menlo Research released in May 2026.

This repository is the public engineering log for the build. Everything I do this summer goes here: CAD modifications, firmware, training data, integration notes, build photos, and the inevitable failures. The goal is for the next student who wants to build a humanoid to have a clearer map than I did.

## The build

| Spec | Value |
|---|---|
| Platform | Asimov v1 (Menlo Research, May 2026) |
| Height | 1.2 m |
| Mass | 35 kg |
| Actuators | 25 ENCOS motors across 5 SKUs |
| Stock compute | Raspberry Pi 5 + Radxa CM5 (Under consideration) |
| Target compute upgrade | NVIDIA Jetson AGX Thor |
| Perception | Stereolabs ZED 2i, Livox Mid-360, Orbbec Gemini 336L |
| Force/torque sensing | Bota Systems SensONE |
| Simulation | MuJoCo, NVIDIA Isaac Sim, Isaac Lab |
| Policy framework | NVIDIA GR00T N1.7, Hugging Face LeRobot |
| 3D printing | Bambu Lab X1C with PA-CF for custom mounts |

## Timeline

- **May 2026:** Kit deposit placed, sponsorship outreach, campaign launch
- **June and July 2026:** MuJoCo simulation work, perception pipeline development
- **August 2026:** Kit arrives, hardware integration, sensor mounting, firmware bring-up
- **September 2026:** Policy training, public demo, complete open-source release

## Setup

Based in West Sussex over the summer. Working between Build Brighton makerspace, a workspace in South London, and my own bench at home in Crawley. A few friends and fellow students from my course will be working alongside me.

## Budget

Total project value: £40,000.

| Line | Cost |
|---|---|
| Asimov v1 kit (with UK VAT and shipping) | £13,000 |
| Sensors (ZED 2i, Mid-360, Gemini 336L, Bota F/T) (Still under consideration) | £6,800 |
| Spare parts (motors die mid build, this isn't optional) | £6,000 |
| Bambu Lab X1C 3D printer for custom mounts | £1,200 |
| Workshop tools | £2,500 |
| Documentation, insurance, customs, makerspace, contingency | £3,500 |
| 3-month project stipend (food and transport; living at parents' so no rent) | £5,000 |
| Unallocated headroom | £1,700 |
| **Total** | **£40,000** |

The Jetson AGX Thor compute upgrade is being pursued separately through NVIDIA's Jetson AI Ambassador programme and is not included in this budget.

Corporate sponsors who donate hardware reduce the cash crowdfund need pound for pound. Any cash surplus over £40k goes into the spares budget.

## How to support

### Crowdfund

GoFundMe campaign: https://www.gofundme.com/f/summer-project-bipedal-humanoid-robot

Backer tiers:

- £10+: name in the final build video credits and on the project sponsors page
- £100+: signed thank you card and access to the private weekly technical email
- £500+: name or logo on the robot
- £1,000+: logo printed at large size on the robot, plus a video call with me at any point during or after the build
- £2,000+: all the above, plus an in-person demo of the finished robot if you are in the UK
- £5,000+: named sponsor in every weekly LinkedIn update for 14 weeks

### Corporate sponsorship

Hardware sponsors receive named credit in every weekly post, co-branded content featuring the sponsored product in use, named placement on the robot itself, and first access for hiring conversations when I graduate.

If your product is on my bill of materials, or is closely relevant to the build, email tharunan19@gmail.com or reach out on LinkedIn.

Current outreach in progress: NVIDIA, Menlo Research, Bambu Lab, Hugging Face, ODrive Robotics, Stereolabs, Orbbec, Livox, Bota Systems, Pollen Robotics, Engineered Arts, FOXTECH, Robotis UK, The Pi Hut, AMD.

## Follow along

Weekly updates every Saturday from now until September:

- LinkedIn: https://www.linkedin.com/in/tharunan-sayanthan-78454a1b8/
- GitHub: this repo

## Repository structure

Coming online as the build progresses:

```
/cad/        Asimov reference CAD modifications (Fusion 360, STEP)
/firmware/   Motor control, sensor integration, low-level firmware
/perception/ Camera, LiDAR, IMU integration code
/sim/        MuJoCo and Isaac Lab models and policies
/training/   Dataset collection, VLA fine-tunes, model cards
/logs/       Weekly write-ups, build photos, failure analysis
/docs/       Reference materials, sourcing notes, troubleshooting
```

## Acknowledgements

Built on top of [Asimov v1 by Menlo Research](https://github.com/asimovinc/asimov-1). All upstream contributions go back to their repository.

Thanks to everyone backing the campaign, sponsoring hardware, or sharing the project. A full sponsor and backer roll appears here as the campaign progresses.

## Contact

Tharunan Sayanthan

tharunan19@gmail.com
https://www.linkedin.com/in/tharunan-sayanthan-78454a1b8/

Open to friends, fellow students, and engineers within commuting distance of South London or Brighton who want to be part of the build. DM on LinkedIn.

## License

The original Asimov v1 work is licensed by Menlo Research under their published terms. Modifications and original code in this repository are released under MIT unless noted otherwise on individual files.
