# Living Brain - Software Engineering Portfolio

> ⚠️ **Disclaimer**
>
> This repository is a personal portfolio showcasing selected work and contributions from my time at **living brain GmbH**.  
> Due to confidentiality, intellectual property and data protection requirements, this repository does **not** contain proprietary source code, internal documentation, patient or customer data, or other confidential company information. The examples of screenshots, videos and descriptions shown here have been carefully selected and are intended to demonstrate my technical experience, responsibilities, and contributions without exposing confidential company information. All rights to the original products, software, assets, trademarks, and other intellectual property remain with their respective owners.

---

## My Role

I joined living brain in 2020 and progressed from an internship to a Senior Software Engineer role.

| Period | Role |
|---|---|
| Sep 2020 - Aug 2021 | **Unity 3D Developer (Internship)** |
| Sep 2021 - Aug 2023 | **Junior Unity Developer** |
| Sep 2023 - Sep 2024 | **Unity Developer** |
| Oct 2024 - Sep 2026 | **Senior Software Engineer** |

During my time at living brain, I worked across software development, product development as well as selected quality and regulatory activities.

I mainly worked with:

C# · Unity 3D · Visual Studio · .NET / WPF · Meta Quest · Pico · Git / GitHub / Plastic SCM · Audacity · Confluence · Jira · Scrum

My work covered:

- Unity 3D software development
- Feature planning, design and implementation
- VR training environments and interactive scenarios
- Audio and sound design, integration and implementation
- Localization and multilingual application support
- Software maintenance and further development
- Internal tools and software libraries
- Debugging and problem solving
- Software documentation
- Technical customer support via email, phone and on-site
- Quality Management, validation and product testing
- Regulatory and medical-device-related activities
- Product testing and audit support
- Organizational and administrative support

---

# Projects

## 1. teora® mind

### Overview

teora® mind is a VR therapy software for cognitive training in clinical rehabilitation and at-home aftercare. It is designed to help people with neurological conditions train cognitive abilities such as memory, attention and concentration through realistic and everyday activities.

Instead of relying primarily on abstract cognitive exercises, teora® mind uses immersive virtual environments to recreate familiar real-world situations. Users can practice activities based on **Activities of Daily Living (ADLs)**, such as preparing coffee, handling groceries or preparing food, in a safe and repeatable environment. The application can be used in conjunction with **teora® platform**, a web-based patient management and therapy management solution that allows therapists to create individual training plans and exchange relevant training data with teora® mind.

The application consists of multiple interactive environments and exercises, including a kitchen, beach and garden, as well as dedicated mini-games. In total, the product includes **17 exercises and 3 mini-games**.

I worked on teora® mind throughout my entire time at living brain, contributing to the development and continuous evolution of the application as a Unity Developer / Software Engineer.

As a medical device, teora® mind was developed within a regulated environment and is a **Class IIa medical device under the European Medical Device Regulation (MDR)**. In addition to software development, I was involved in quality management and regulatory activities, including software validation, product testing, documentation, QMS changes, and the planning, preparation and support of internal and external audits.

### General Work

Across the different environments and exercises of teora® mind, I was regularly involved in the implementation and setup of new and existing scenes.

This included:  
- Implementing and maintaining **level and scene structures**, including colliders, respawn areas and scene-specific setup
- Developing and maintaining the **in-game tablet UI** and its application-wide features
- Editing, integrating and configuring **audio and sound systems** across scenes and interactive objects
- Implementing and maintaining **localization** with multilanguage content, including texts, assets, a language selection and right-to-left (RTL) support
- Supporting **multiple VR headsets**, including Meta Quest 2, Quest 3S and Pico 4
- Implementing and adapting **VR interaction and UI systems**, including pointers, raycasts and controller-specific UI hints
- Developing reusable and configurable systems and components using **ScriptableObjects** and **Prefabs**
- Implementing application-wide features such as **pause tracking, scene transitions and device status information**
- Integrating features for communication with **teora® platform** and other parts of the teora® ecosystem
- Adapting and reworking existing gameplay and interaction systems to new environments
- Collaborating with artists to integrate and iterate on visual effects and gameplay feedback
- Updating Unity and project packages while maintaining compatibility with existing systems
- Supporting **testing, debugging, bug fixing and quality assurance** throughout development within a regulated medical-device environment

### Selected Work

#### 1. Minigame Shooting (Prototype)

I developed gameplay features and interactive systems for a shooting-based VR minigame. This level was still under development and was not completed as a finished product.

The prototype combines shooting mechanics, interactive objects, physics-based interactions and timed gameplay events into a playable VR experience. In each playthrough the targets spawn at random locations which makes every playthrough unique.

**My contribution included:**
- Developing the **scoring and timer systems**, including difficulty-dependent timing and a wave-based level completion condition
- Implementing the **nailgun interaction and shooting feedback**, including projectile particle trails
- Developing interactive shootables and their individual behaviors, including:
  - **Moving robot** following a defined path
  - **Jack-in-the-box** with opening/closing lid, physics-based jumping behavior as well as reactions when hit
  - **Ice block** with hit feedback and progressive crack decals
  - **Balloons** with spawning, movement, scaling and hit effects
  - **UFO shield** with projectile interaction and visual hit feedback
- Implementing the **Freeze Event**, temporarily pausing affected gameplay objects through their physics state

<video src="https://github.com/user-attachments/assets/ae4ec8d4-c3bb-41bc-b841-8bbba5957583.mp4"></video>

#### 2. Tutorial Rework

The existing tutorial flow was completely replaced with a new concept consisting of a guided tutorial and a separate recycling section. We wanted to provide a clearer and more accessible introduction to the VR application.

The result was a more structured onboarding experience that gradually introduced users to the application's interactions and mechanics.

**My contribution:**
- Reworked the existing **gameplay and scene structure**
- Extended and adapted the existing **quest system**
- Adapted existing **interaction logic** to the new gameplay flow
- Programmatically integrated and controlled the **wooden block animations**, including forward and reverse playback triggered by gaze targeting
- Implemented new **UI panels and visual guidance** in collaboration with artists, including controller guidance UI

<video src="https://github.com/user-attachments/assets/67d8dc8f-a996-40ad-a3bd-c99e67235243.mp4"></video>

#### 3. Custom Sound System

I worked closely with another developer on the sound system used throughout teora® mind. While the underlying system was developed by my colleague, we collaborated on its design and integration into the application. The system used a material-based sound matrix with **50+ sound combinations**, covering different material interactions for collision sounds as well as grab and snap sounds for interactable objects.

Particular attention was given to creating believable audio feedback for different materials and interactions, helping to make physical interactions in VR feel more natural and immersive.

**My contribution:**
- Researched and selected **suitable sound effects**, including lots of material-specific sounds
- Edited and prepared **audio assets using Audacity**
- Established **workflows and naming conventions** for organizing and integrating audio assets
- Integrated and configured **sound components across scenes and reusable prefabs**
- Continuously **maintained and extended** the audio setup as new content was added

In the video below, different collision sounds can be heard for materials such as **glass, stone, plastic and metal**. The sound feedback also adapts dynamically based on the intensity of the collision.

<video src="https://github.com/user-attachments/assets/9bb1cf9e-b63a-4fa2-9469-746347fc20fa.mp4"></video>

#### 4. Localization

I contributed to the implementation and expansion of the localization system used throughout teora® mind. The system supported localized UI texts and assets across the application, including dynamic content generated at runtime, and was designed to support **12 languages**.

**My contribution:**
- Created and maintained **String Tables and Asset Tables** for multilingual content
- Integrated and maintained **localized UI texts across the application**
- Developed solutions for **dynamic localized strings**, allowing values generated at runtime, such as calculated amounts, to be inserted into localized text
- Implemented a **custom currency formatter** for use with Unity's Smart Strings
- Developed localization support for **non-text assets**, including localized materials
- Implemented and integrated the **language selection UI and its interaction**
- Contributed to the integration and maintenance of **right-to-left (RTL) language support**
- Established reusable workflows and structures for managing localized content across the application

The video below shows different UI elements updating when switching between languages. Towards the end, it also demonstrates RTL support, including mirrored tablet layouts and UI elements adapted to the right-to-left reading direction.

<video src="https://github.com/user-attachments/assets/6c2eb8e6-06c5-40f6-b7e7-e75d01304861.mp4"></video>

The screenshot shows different assets with localized materials that are automatically switched based on the selected language.

<img width="750" alt="teora_localized_assets" src="https://github.com/user-attachments/assets/092bee8b-1d1a-4aa6-87e3-19cfee5cdbea"/>

#### 5. Custom Cable System for Kitchen Coffee Machine

For the kitchen environment, I developed a custom physics-based cable system to replace the previously used third-party plugin. <br>
The goal was to reduce external dependencies while having more control over the system and its behavior.

**My contribution:**
- Designed and implemented the cable system using **Unity physics, rigidbodies and joints**
- Created the **cable mesh procedurally** based on the physical cable structure
- Integrated the system with existing VR interactions
- Designed the cable behavior with **user experience in mind**, including automatic retraction when the cable is stretched too far
- Tested and evaluated the **performance using Meta's OVR Metrics Tool** in comparison to the previously used third-party plugin

<video src="https://github.com/user-attachments/assets/9226f276-97a0-4a33-9236-449ce288868a.mp4"></video>
---

## 2. teora® body

### Overview

teora® body is a VR application for **upper-extremity movement training**, with a focus on functional movements of the shoulder and elbow. It uses interactive exercises to train mobility, strength and coordination in a motivating way.

Unlike teora® mind, which primarily focuses on cognitive training, teora® body uses **hand tracking** to allow users to interact with the virtual environment using their hands instead of traditional VR controllers.

The application combines several interactive exercises, including activities such as inflating balloons and controlling a rocket. In total, the application includes **6 exercises**.

I worked on teora® body from November 2024 to July 2025, contributing to the development of the application from the initial project setup through the implementation and refinement of its interactive exercises.

My work focused particularly on **hand tracking integration, VR interactions, reusable systems, UI and gameplay**, as well as localization, audio and general application maintenance.

### General Work

Throughout the development of teora® body, I worked on shared systems and features required across the different exercises and environments.
This included:

- Integrating and adapting **Meta XR Core SDK and Meta XR Interaction SDK** for hand tracking
- Developing and maintaining **hand-based interactions**, including touch, grab and lever interactions
- Creating and maintaining **reusable prefabs and interaction components** for use across multiple exercises
- Reworking the **in-game tablet and UI** for hand-based interaction
- Integrating and maintaining **localization**, including right-to-left (RTL) support and localized assets
- Editing, integrating and configuring **audio and sound systems** across scenes and interactive objects
- Updating Unity and project packages while maintaining compatibility with existing systems
- Supporting **testing, debugging, bug fixing and quality assurance** throughout development

### Selected Work

#### Interactions & Exercises

This video provides an overview of several interactive exercises in teora® body and some of the systems I worked on throughout the application:
- **Hand Tracking and tablet interaction**, including localized UI content
- **Rocket Guiding**: implemented the fading out of the small planet when the rocket starts, the visual rope belonging to the rocket, its color feedback, sound as well as collectables visual cue (speechbubble), contributed to the hover button and astronaut animations and general interaction design
- **Inflating Balloons**: contributed to the interactive balloon inflation, including different outcomes when balloons are released and flying away or when balloons are overinflated and pop
- **Ice Cream Stacking**: catching and stacking objects to build a complete ice cream tower, reworked the mechanics to work with hand tracking, implemented spawn system and the shadows of falling items
- **Chain Smashing**: physically interacting with and breaking incoming objects on a conveyor belt, reworked the mechanics to work with hand tracking, implemented conveyor belt movement with texture offset, integrated point system and its displays

<video src="https://github.com/user-attachments/assets/ce1a8ba6-500f-42b8-8909-6e0496386ce1.mp4"></video>

---

## 3. Device Setup Tool

### Overview

The Device Setup Tool is an internal **WPF desktop application** developed to prepare and configure VR devices for use within the teora® ecosystem.

It is used to set up device-specific metadata required for features such as **streaming with teora® supervisor** and integration with **teora® platform**, where devices need to be uniquely associated with their intended use. The goal was to provide a **clean and quick setup process for every VR device before shipping to customers**.

I developed the tool and was responsible for its implementation, maintenance and testing.

### My Contribution

- Developed the application using **.NET and WPF**
- Implemented communication with VR devices using **Android Debug Bridge (ADB)**
- Implemented automated tests using **NUnit**
- Maintained and extended the tool as requirements evolved

<video src="https://github.com/user-attachments/assets/55114b43-09b2-4933-b481-38385b7157e0.mp4"></video>

---
