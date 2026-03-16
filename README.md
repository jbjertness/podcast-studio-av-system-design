# Podcast Studio Broadcast System Design
This project documents a proposed audio, video, networking, and lighting architecture for a flexible multi-purpose production environment consisting of a studio, live room, and event hall.

I designed this system with an emphasis on modularity, and as a result upports a variety of production scenarios including:

- Podcast recording
- Music Production
- Live streaming
- Remote Production
- Multi-camera broadcast production
- Remote guest integration

The system leverages modern broadcast and AV technologies such as Dante, NDI, POE, and 12gSDI to create a scalable and adaptable production workflow.

## System Overview

The studio supports:
The studio is designed around a centralized production control room that manages audio mixing, video switching, recording, and live streaming for an attached live room and seperated event space. 

![Studio System Diagram](images/studio-system-diagram.png)

## Audio System
The audio system is centered around the Allen & Heath SQ-5 digital mixer with Dante networking for flexible routing between rooms.

Components
- Allen & Heath SQ-5 mixer with 32x32 Dante I/O
- Dedicated PoE Dante network switch
- Dante boundary microphones for event hall capture
- Dante integration with Tesira Forte DSP
- Talkback paging system
- Audio wall plate connectivity from studio control room to live room

## Video System
Video production is powered by the Blackmagic ATEM production ecosystem, which supports 12gSDI switching, recording, and streaming.

Components
- ATEM 4 M/E Constellation 4K video switcher
- ATEM 1 M/E Advanced Panel 20 control surface
- vMix streaming and recording workstation
- Elgato Stream Deck controller

Camera system
- 3× BirdDog P120 Full NDI PTZ cameras
- Magewell NDI-to-SDI converters
- PTZOptics SuperJoy camera controller

The system supports NDI camera feeds from the event hall to the studio control room.

## Podcast Production System

Components
- RedNet AM2 Dante headphone interfaces
- Dedicated podcast monitoring displays
- Remote guest video interaction system
- Integrated webcam solution

Audio from remote participants is routed through the SQ-5 and returned to the monitoring interfaces for hosts.

## Lighting System for Studio

Equipment
- CHAUVET COLORdash PAR H18X RGBWA+UV wash lights
- ETC ColorSource AV 20 lighting console
- CHAUVET OnAir IP LED soft lights

Lighting is controlled through DMX patch panels distributed across the studio and live room, allowing flexible lighting layouts.

## Production Workstation
Custom workstation designed for demanding video effects and 4k multi-stream recording and 12bit 4:4:4 color depth. 

Our configuration
- Intel i9-13900K CPU
- RTX 4080 Super GPU for AV1 encoding
- Blackmagic DeckLink 8K Pro capture card
- NVMe storage array for high-bitrate recording
- ASUS ProArt Z790 Creator motherboard

The workstation runs vMix production software for recording and streaming.

## Power Protection

UPS Battery backup
Power Conditioning Unit

## Technology Used

- diagrams.net (draw.io)
- Dante audio networking
- NDI Video Networking
- 12G SDI Broadcast Video
- Biamp Tesira Software
- NDI
- vMix
- Reaper
- Dante audio networking

